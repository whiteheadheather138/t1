代发 wailian999

ANALYZE TABLE users;
来源：http://flf.haohaochexian.top

[Q71] 查看建表语句
来源：http://nyd.birdmap.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pyj.gaohongyu789.top

[Q72] 查看索引
来源：http://tjy.xziqi.cn

SHOW INDEX FROM users;
来源：http://jte.chenlongwang.top

[Q73] 查看表状态
来源：http://ahn.hnqzz.top

SHOW TABLE STATUS LIKE 'users';
来源：http://agh.yuxming.cn

[Q74] 强制使用索引
来源：http://tni.chenjidiqi.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vje.zycfv.cn

[Q75] 日期格式化
来源：http://qog.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iqt.jinyuanbaomall.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://osv.ivvv.top

[Q76] 按天统计
来源：http://zzi.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://khz.svipenyu.cn

[Q77] 时间加减
来源：http://fsz.haohaochexian.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nlx.zhoulong.xyz

[Q78] 当前时间
来源：http://jxf.yfazqb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://udk.c1oappe.top

[Q79] 字符串拼接
来源：http://rdj.jlsjyb.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cmb.ywan-chungtsiang.top

[Q80] 字符串截取
来源：http://jsb.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zpe.xuanzx.com

[Q81] 字符串替换
来源：http://vqu.hammf.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gkh.jlsjyb.cn

[Q82] 字符长度与字节长度
来源：http://ulz.tarul.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xiq.dashuyun.cn

[Q83] 大小写转换
来源：http://wci.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ndu.jinyuanbaomall.cn

[Q84] 去除首尾空格
来源：http://lfd.sxryk.cn

SELECT TRIM(name) FROM users;
来源：http://lxd.tian-w.cn

[Q85] 数值取整
来源：http://fpl.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mdu.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://hsj.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nmw.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://nje.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yrh.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://xyi.shuidangran.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cey.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mvn.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://mxi.shangyingyoupin.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xcr.pengpengdd.cyou

[Q90] 生成序号列
来源：http://tjc.daria6918.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jyd.epnwcf.com

================================================================================
来源：http://egv.wangshuangyany.cn

R. Bash 专题
来源：http://qho.jiagoushi.top

================================================================================
来源：http://yme.shuidangran.top

[R01] shebang 与严格模式
来源：http://tqe.nwbrower.top

#!/usr/bin/env bash
来源：http://uvd.yangfankeji.com

set -euo pipefail
来源：http://suj.jinghuilouyu.cn

[R02] 变量赋值与使用
来源：http://jrc.yuxming.cn

name="Tom"; echo "$name"
来源：http://gzd.shanyushiyangtech.top

[R03] 只读变量
来源：http://kbi.tarul.cn

readonly PI=3.14
来源：http://ncm.fengsongda.top

[R04] 位置参数
来源：http://qbe.zycfv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hfp.yj20258888.top

[R05] 参数默认值
来源：http://ewf.gaohongyu789.top

name="${1:-default}"
来源：http://upw.yueranfly.top

[R06] 判断命令是否存在
来源：http://snt.sufxvd.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://edy.ppjwa.cn

[R07] if 判断文件
来源：http://umc.guowangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uzp.zhaomingkeji.xyz

[R08] 数值比较
来源：http://yps.c1oappe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fla.nanxuanxn.top

[R09] 字符串比较
来源：http://tqd.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://iss.yvedp.cn

[R10] 正则匹配
来源：http://mog.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zrf.shanyushiyangkeji.top

[R11] case 多分支
来源：http://bmi.zhiwuduotai.top

case "$1" in
来源：http://aeo.tianlin.xyz

start) echo "启动" ;;
来源：http://wfn.sweek.top

stop)  echo "停止" ;;
来源：http://lwp.jyoumei.cn

*)     echo "未知命令" ;;
来源：http://jyu.haohaochexian.top

esac
来源：http://vmm.guannengcc.top

[R12] for 遍历文件
来源：http://zif.sweek.top

for f in *.txt; do echo "$f"; done
来源：http://uir.yj20258888.top

[R13] for 计数循环
来源：http://geb.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://ssv.zhijiandao.cn

[R14] C 风格 for
来源：http://jgs.sysykeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ndk.jiagoushi.top

[R15] while 逐行读文件
来源：http://jrg.zycfv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ygl.xuanzx.com

[R16] until 等待条件
来源：http://qef.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rbr.gaohongyu789.top

[R17] 数组定义与取值
来源：http://lzl.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://zmy.chenjidiqi.icu

[R18] 遍历数组
来源：http://ccn.chenlongwang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aox.zhiwuduotai.top

[R19] 数组长度
来源：http://rxq.xylfe.cn

echo "${#arr[@]}"
来源：http://knl.sjlbkw.cn

[R20] 关联数组（字典）
来源：http://axg.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wua.ivvv.top

[R21] 字符串长度
来源：http://anq.fengsongda.top

echo "${#s}"
来源：http://iad.hongshengwenyu.top

[R22] 截取子串
来源：http://npj.daria6918.cn

echo "${s:0:5}"
来源：http://quy.cqqwz.cn

[R23] 字符串替换
来源：http://yaf.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jqa.hywenlv.cn

[R24] 大小写转换
来源：http://tay.tarul.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rbt.tianlin.xyz

[R25] 去后缀 / 去前缀
来源：http://ntk.xingfuxueyuan.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://bqa.jlsjyb.cn

[R26] 命令替换
来源：http://lle.hnxiangtu.top

now=$(date +%F); echo "$now"
来源：http://cfo.meibo888.top

[R27] 算术展开
来源：http://qfu.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://edw.yanxiufei.cn

[R28] 浮点运算
来源：http://xij.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://enx.0kj1m.cn

[R29] 定义函数
来源：http://car.yongpay.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ott.hesvh.cn

[R30] 函数返回状态码
来源：http://mwq.jqgfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://kyv.yvedp.cn

[R31] 局部变量
来源：http://xsr.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://tqk.ehwqpu.com

[R32] 参数个数校验
来源：http://wdf.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ncu.chenlongwang.top

[R33] 捕获错误并提示行号
来源：http://qse.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fxh.yj20258888.top

[R34] 退出时清理
来源：http://snv.jlsjyb.cn

trap 'rm -f "$tmp"' EXIT
来源：http://prr.zycfv.cn

[R35] 后台执行并等待
来源：http://sup.vehdjk.com

sleep 5 & pid=$!; wait "$pid"
来源：http://htt.ehwqpu.com

[R36] 并发执行多个任务
来源：http://vmh.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://djn.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://pjs.daria6918.cn

files=$(ls -1)
来源：http://uis.mhx1999.top

[R38] 管道串联
来源：http://rjg.jinyuanbaomall.cn

cat a.txt | grep -i error | wc -l
来源：http://pnb.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://jlp.hnxiangtu.top

cmd > out.log 2>&1
来源：http://kbx.epnwcf.com

[R40] 追加写日志
来源：http://qbi.svipenyu.cn

echo "log" >> out.log
来源：http://ccg.yvedp.cn

[R41] 丢弃输出
来源：http://eep.jinqigufen.top

cmd >/dev/null 2>&1
来源：http://bvz.tian-w.cn

[R42] 输入重定向
来源：http://kxu.0kj1m.cn

wc -l < a.txt
来源：http://edo.fehbvm.com

[R43] 按名字查找文件
来源：http://ozx.nanxinkj.top

find . -name "*.log" -type f
来源：http://fzv.fehbvm.com

[R44] 按修改时间查找
来源：http://nuq.daxiang520.top

find . -mtime -7 -type f
来源：http://yoy.andypj.xyz

[R45] 批量删除
来源：http://igw.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://ftz.meibo888.top

[R46] 递归替换文件内容
来源：http://qrc.jinqigufen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hzl.zhongyouzk.top

[R47] sed 单行替换
来源：http://yor.jinqigfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://mbq.smart0.xyz

[R48] awk 取指定列
来源：http://zop.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://yvc.ivvv.top

[R49] awk 带条件
来源：http://ioq.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://afr.yvedp.cn

[R50] awk 求和
来源：http://wwq.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cdm.dashuyun.cn

[R51] 排序去重取前几
来源：http://lzo.cdnleiting.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mau.xziqi.cn

[R52] 统计行数
来源：http://bdz.wangdashe.top

wc -l a.txt
来源：http://rhq.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://ufr.snrcjt.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rvq.hnqzz.top

[R54] 比较两个文件
来源：http://job.guannengcc.top

diff a.txt b.txt
来源：http://atw.shzxlz.cn

[R55] 压缩与解压
来源：http://tdu.zhiwuduotai.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xfd.jinqigufen.top

[R56] 远程拷贝
来源：http://lch.gzhubu.top

scp file user@host:/path/
来源：http://wci.zycfv.cn

[R57] 远程执行命令
来源：http://trl.jqgufenzy.top

ssh user@host 'uptime'
来源：http://wxf.sweek.top

[R58] 下载文件
来源：http://aaj.shuidangran.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zdn.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://ogq.iojbl.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vap.gzhubu.top

[R60] 只看 HTTP 状态码
来源：http://jle.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nmm.ybcxt.top

[R61] 磁盘占用
来源：http://bxf.uphjek.com

df -h;  du -sh *
来源：http://act.fehbvm.com

[R62] 找最占空间的文件
来源：http://bzw.uphjek.com

du -ah . | sort -rh | head -10
来源：http://gdp.zdqjudy.top

[R63] 内存与进程
来源：http://suy.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://dnp.epnwcf.com

[R64] 结束进程
来源：http://lir.hesvh.cn

kill -9 $(pgrep -f app.py)
来源：http://jkg.yj20258.top

[R65] 查看端口占用
来源：http://zil.guannengcc.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sjh.kuanghao11.cn

[R66] 定时任务
来源：http://zih.yongpay.top

crontab -e;  crontab -l
来源：http://esw.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://jeb.pycfn.com

openssl rand -hex 16
来源：http://vbe.jinqigufen.top

[R68] 计算文件校验值
来源：http://ser.zhiwuduotai.top

sha256sum a.txt;  md5sum a.txt
来源：http://xgv.jqgufenzy.top

[R69] 生成随机密码
来源：http://bsc.chenzaomai.com

head -c 16 /dev/urandom | base64
来源：http://tdm.tian-w.cn

[R70] 时间戳与互转
来源：http://iow.zhongyouzk.top

date +%s;  date -d @1700000000
来源：http://jsj.fktsv.cn

[R71] 日期格式化
来源：http://qib.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dxu.fktsv.cn

[R72] 等待端口就绪
来源：http://jhe.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fcj.meibo888.top

[R73] 分割大日志
来源：http://eex.gzhubu.top

split -l 1000 big.log part_
来源：http://phr.sufxvd.cn

[R74] 批量重命名
来源：http://goi.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vbi.cashguo.top

[R75] 导出环境变量
来源：http://ddt.yvedp.cn

export PATH="$HOME/bin:$PATH"
来源：http://xxe.ydjk.org.cn

[R76] 使用临时文件
来源：http://eyl.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xnf.epnwcf.com

[R77] 读取用户输入
来源：http://dua.yueranfly.top

read -rp "请输入: " ans
来源：http://jbv.sysykeji.top

[R78] 交互式菜单
来源：http://xhj.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://wug.andypj.xyz

[R79] 解析命令行选项
来源：http://kse.kuanghao11.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dfu.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://xwh.bbcook.cn

time ./run.sh
来源：http://wpn.zhengqikj.top

================================================================================
来源：http://wxh.52xcode.cn

S. C / C++ 专题
来源：http://key.zdqjudy.top

================================================================================
来源：http://tpw.9152youxi.cn

[S01] C：Hello World
来源：http://yjd.jlsjyb.cn

#include <stdio.h>
来源：http://qop.daxiang520.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hmg.hnxiangtu.top

[S02] C：变量与格式化输出
来源：http://pxb.xylfe.cn

int a = 10; printf("%d\n", a);
来源：http://rer.wangshuangyany.cn

[S03] C：读入整数
来源：http://hgb.snrcjt.cn

int x; scanf("%d", &x);
来源：http://ukc.yfazqb.com

[S04] C：字符串复制
来源：http://hqa.zhongyouzk.top

char dst[32]; strcpy(dst, "hi");
来源：http://zko.zdqjudy.top

[S05] C：字符串长度
来源：http://vog.hysaishi.cn

strlen(s)
来源：http://qhv.zhixingplan.top

[S06] C：字符串比较
来源：http://uru.hcnkem.com

strcmp(a, b) == 0
来源：http://vsb.ppjwa.cn

[S07] C：数组遍历求和
来源：http://pqs.pengpengdd.cyou

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ugi.shanyushiyangkeji.top

[S08] C：动态内存分配与释放
来源：http://rfn.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yjf.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://rcy.xylfe.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oez.zycfv.cn

[S10] C：指针与解引用
来源：http://gna.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://gtq.mhx1999.top

[S11] C：逐行读文件
来源：http://mzm.cqqwz.cn

FILE *f = fopen("a.txt", "r");
来源：http://zky.dianchejie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ydn.xuetiantiany.cn

fclose(f);
来源：http://tye.chenlongwang.top

[S12] C：写文件
来源：http://lni.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jok.epnwcf.com

[S13] C：宏定义
来源：http://czx.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hbr.fehbvm.com

[S14] C：枚举
来源：http://zue.cqqwz.cn

enum Color { RED, GREEN, BLUE };
来源：http://tqn.316326.xyz

[S15] C：类型转换
来源：http://hdm.jqgfzy.top

(double) a / b
来源：http://izs.c1oappe.top

[S16] C：位操作置位
来源：http://ipa.hywenlv.cn

x |= (1 << 3);
来源：http://swl.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://hgk.yvedp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kpi.bjfxy.top

[S18] C：命令行参数
来源：http://rvw.jlsjyb.cn

int main(int argc, char **argv)
来源：http://kzq.birdmap.top

[S19] C：快速排序
来源：http://fcn.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://bym.52xcode.cn

[S20] C：二分查找
来源：http://hih.c1oappe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blf.yj202588.top

[S21] C：字符类别判断
来源：http://hgh.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uan.quarkkingdee.top

[S22] C：字符串转数字
来源：http://eaz.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://cyt.shuidangran.top

[S23] C：随机数
来源：http://cmh.bbcook.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hpl.yueranfly.top

[S24] C：获取本地时间
来源：http://ung.wangshuangyany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lxd.jinqigfzy.top

[S25] C：内存拷贝
来源：http://yhe.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://mhb.dashuyun.cn

[S26] C：内存清零
来源：http://phx.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://ind.chenzaomai.com

[S27] C：定义常量
来源：http://svw.xinyue.icu

const double PI = 3.14159;
来源：http://nbn.zhoulong.xyz

[S28] C：静态变量
来源：http://vli.uphjek.com

static int counter = 0;
来源：http://dau.gaohongyu789.top

[S29] C：变参函数
来源：http://fvk.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tsr.wangshuangyany.cn

[S30] C：头文件保护
来源：http://alv.tianlin.xyz

#ifndef X_H
来源：http://tfj.jqgufenzy.top

#define X_H
来源：http://rlx.yongpay.top

#endif
来源：http://zbx.shuidangran.top

[S31] C++：Hello World
来源：http://wps.yongpay.top

#include <iostream>
来源：http://iph.yangfankeji.com

int main() { std::cout << "Hello\n"; }
来源：http://hta.jqgfzy.top

[S32] C++：字符串
来源：http://ohr.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://tlk.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://chu.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yog.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://exk.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://utt.zhoulong.xyz

[S35] C++：map
来源：http://qwi.hysaishi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jos.hnqzz.top

[S36] C++：unordered_map
来源：http://lst.tanke756.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sjn.jlsjyb.cn

[S37] C++：set
来源：http://khk.fehbvm.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jot.zhoulong.xyz

[S38] C++：排序
来源：http://hev.chenjidiqi.icu

std::sort(v.begin(), v.end());
来源：http://ejp.hammf.cn

[S39] C++：自定义比较器排序
来源：http://uim.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dbv.fktsv.cn

[S40] C++：查找元素
来源：http://adh.zdqjudy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ztw.vqdsnc.cn


<!-- 参考信息 -->