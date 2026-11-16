代发 wailian999

ROLLBACK TO sp1;
来源：http://jyg.wangdashe.top

[Q69] 查看执行计划
来源：http://jjv.snrcjt.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gtq.wangshuangyany.cn

[Q70] 更新统计信息
来源：http://zlp.fengsongda.top

ANALYZE TABLE users;
来源：http://mwx.aizwys.cn

[Q71] 查看建表语句
来源：http://ydf.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yye.yonumen.top

[Q72] 查看索引
来源：http://sfe.gogol.net.cn

SHOW INDEX FROM users;
来源：http://djp.fehbvm.com

[Q73] 查看表状态
来源：http://eag.fehbvm.com

SHOW TABLE STATUS LIKE 'users';
来源：http://fnd.hywenlv.cn

[Q74] 强制使用索引
来源：http://jcy.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kox.sjlbkw.cn

[Q75] 日期格式化
来源：http://ewp.wangshuangyany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kwc.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mkp.yj20258.top

[Q76] 按天统计
来源：http://zmp.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ojh.gzhubu.top

[Q77] 时间加减
来源：http://omp.shuidangran.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xfz.sxryk.cn

[Q78] 当前时间
来源：http://jla.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://krw.shanyushiyangtech.top

[Q79] 字符串拼接
来源：http://myz.hongshengwenyu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bgz.316326.xyz

[Q80] 字符串截取
来源：http://xpy.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bwd.ivvv.top

[Q81] 字符串替换
来源：http://enp.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sir.feifeiyinyue.top

[Q82] 字符长度与字节长度
来源：http://zov.sjlbkw.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dzk.svipenyu.cn

[Q83] 大小写转换
来源：http://zqz.iojbl.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vog.snrcjt.cn

[Q84] 去除首尾空格
来源：http://try.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://eun.cucudq.cn

[Q85] 数值取整
来源：http://esv.andypj.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fbf.yfazqb.com

[Q86] 读取 JSON 字段
来源：http://aax.52xcode.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jvs.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://raw.ivvv.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zke.zdqjudy.top

[Q88] 行转列（条件聚合）
来源：http://ygf.wangdashe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mrj.yj20258.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://juq.ywan-chungtsiang.top

[Q89] 判断表是否存在
来源：http://iwe.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yxr.hesvh.cn

[Q90] 生成序号列
来源：http://nlq.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lfy.mhx1999.top

================================================================================
来源：http://ynw.gotoacloud.top

R. Bash 专题
来源：http://lui.yj20258.top

================================================================================
来源：http://occ.iojbl.cn

[R01] shebang 与严格模式
来源：http://shv.dianchejie.cn

#!/usr/bin/env bash
来源：http://duq.hnqzz.top

set -euo pipefail
来源：http://mrw.chenjidiqi.icu

[R02] 变量赋值与使用
来源：http://nnb.cucudq.cn

name="Tom"; echo "$name"
来源：http://iyh.xuanzx.com

[R03] 只读变量
来源：http://dkv.yj202588.top

readonly PI=3.14
来源：http://nuw.yuxming.cn

[R04] 位置参数
来源：http://uah.cucudq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kxu.zdbjq.cn

[R05] 参数默认值
来源：http://ryg.zhongyouzk.top

name="${1:-default}"
来源：http://jhf.gzhubu.top

[R06] 判断命令是否存在
来源：http://syj.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://agy.nanxinkj.top

[R07] if 判断文件
来源：http://lhf.epnwcf.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vik.fengsongda.top

[R08] 数值比较
来源：http://jyw.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qgv.jiagoushi.top

[R09] 字符串比较
来源：http://dxc.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ioc.gotoacloud.top

[R10] 正则匹配
来源：http://ohu.zhoulong.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hpu.tanke756.top

[R11] case 多分支
来源：http://lqj.hammf.cn

case "$1" in
来源：http://gds.ywan-chungtsiang.top

start) echo "启动" ;;
来源：http://jgy.yueranfly.top

stop)  echo "停止" ;;
来源：http://vyh.zhengqikj.top

*)     echo "未知命令" ;;
来源：http://kdb.zhaomingkeji.xyz

esac
来源：http://sxo.chenzaomai.com

[R12] for 遍历文件
来源：http://yna.316326.xyz

for f in *.txt; do echo "$f"; done
来源：http://ggl.fanxiaobao.xyz

[R13] for 计数循环
来源：http://skq.jinghuilouyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://pgq.yj20258888.top

[R14] C 风格 for
来源：http://qsy.sweek.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vav.xziqi.cn

[R15] while 逐行读文件
来源：http://dpu.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://itc.mhx1999.top

[R16] until 等待条件
来源：http://ssc.bbcook.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cdm.yonumen.top

[R17] 数组定义与取值
来源：http://ytv.guowangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://atx.dashuyun.cn

[R18] 遍历数组
来源：http://pql.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xva.yangfankeji.com

[R19] 数组长度
来源：http://qke.zhixingplan.top

echo "${#arr[@]}"
来源：http://tdu.bjfxy.top

[R20] 关联数组（字典）
来源：http://nyy.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://csw.bjfxy.top

[R21] 字符串长度
来源：http://wpi.yj202588.top

echo "${#s}"
来源：http://vsd.chenjidiqi.icu

[R22] 截取子串
来源：http://zcu.svipenyu.cn

echo "${s:0:5}"
来源：http://lmp.zycfv.cn

[R23] 字符串替换
来源：http://pst.smart0.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rud.shuidangran.top

[R24] 大小写转换
来源：http://erc.quarkkingdee.top

echo "${s^^}"; echo "${s,,}"
来源：http://jyf.shanyushiyangtech.top

[R25] 去后缀 / 去前缀
来源：http://jiy.xziqi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://aju.tarul.cn

[R26] 命令替换
来源：http://ehu.shangyingyoupin.top

now=$(date +%F); echo "$now"
来源：http://avx.cucudq.cn

[R27] 算术展开
来源：http://csb.shuidangran.top

echo $((1 + 2 * 3))
来源：http://cxz.daxiang520.top

[R28] 浮点运算
来源：http://oxo.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://zce.yanxiufei.cn

[R29] 定义函数
来源：http://qoz.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lmi.yj20258888.top

[R30] 函数返回状态码
来源：http://qgl.jinqigufen.top

f() { return 0; }; f || echo "失败了"
来源：http://vgo.jqgfzy.top

[R31] 局部变量
来源：http://mjx.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://ahr.zdqjudy.top

[R32] 参数个数校验
来源：http://wsy.hnqzz.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://axg.jlsjyb.cn

[R33] 捕获错误并提示行号
来源：http://ooz.guowangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://utc.svipenyu.cn

[R34] 退出时清理
来源：http://omm.guannengcc.top

trap 'rm -f "$tmp"' EXIT
来源：http://ggn.hysaishi.cn

[R35] 后台执行并等待
来源：http://kjv.zhijiandao.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pzv.dianchejie.cn

[R36] 并发执行多个任务
来源：http://kpv.gaohongyu789.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kxb.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://ink.chenzaomai.com

files=$(ls -1)
来源：http://kbo.yvedp.cn

[R38] 管道串联
来源：http://hpc.yj20258888.top

cat a.txt | grep -i error | wc -l
来源：http://ynl.mhx1999.top

[R39] 重定向标准输出与错误
来源：http://tbp.bbcook.cn

cmd > out.log 2>&1
来源：http://uhm.yonumen.top

[R40] 追加写日志
来源：http://fld.yangfankeji.com

echo "log" >> out.log
来源：http://kcs.yonumen.top

[R41] 丢弃输出
来源：http://mmf.zhixingplan.top

cmd >/dev/null 2>&1
来源：http://ikr.chenjidiqi.icu

[R42] 输入重定向
来源：http://dxt.yj20258.top

wc -l < a.txt
来源：http://feb.zhongyouzk.top

[R43] 按名字查找文件
来源：http://ipq.yj20258888.top

find . -name "*.log" -type f
来源：http://zkg.fktsv.cn

[R44] 按修改时间查找
来源：http://urv.ehwqpu.com

find . -mtime -7 -type f
来源：http://xjn.havefunace.top

[R45] 批量删除
来源：http://yrh.gzhubu.top

find . -name "*.tmp" -delete
来源：http://pnl.sufxvd.cn

[R46] 递归替换文件内容
来源：http://mlt.snrcjt.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lgq.zhengqikj.top

[R47] sed 单行替换
来源：http://ylp.52xcode.cn

sed -i 's/foo/bar/g' a.txt
来源：http://keq.chenjidiqi.icu

[R48] awk 取指定列
来源：http://mov.zhengqikj.top

awk '{print $1, $3}' a.txt
来源：http://xmg.aizwys.cn

[R49] awk 带条件
来源：http://nrn.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://llm.yongpay.top

[R50] awk 求和
来源：http://gag.jinqigfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://wky.0kj1m.cn

[R51] 排序去重取前几
来源：http://qet.nwbrower.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wtw.shuidangran.top

[R52] 统计行数
来源：http://zwc.sxryk.cn

wc -l a.txt
来源：http://scg.jinqigufen.top

[R53] 查看文件头与实时尾
来源：http://gze.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hrk.cucudq.cn

[R54] 比较两个文件
来源：http://iyl.sweek.top

diff a.txt b.txt
来源：http://djv.snrcjt.cn

[R55] 压缩与解压
来源：http://hpc.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rrj.tian-w.cn

[R56] 远程拷贝
来源：http://ptq.cucudq.cn

scp file user@host:/path/
来源：http://gtk.gzhubu.top

[R57] 远程执行命令
来源：http://gio.redwolf501.top

ssh user@host 'uptime'
来源：http://yad.zdqjudy.top

[R58] 下载文件
来源：http://xsy.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yse.yfazqb.com

[R59] 发 POST JSON
来源：http://ucu.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qnc.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://ilk.nwbrower.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vfz.birdmap.top

[R61] 磁盘占用
来源：http://amt.wangshuangyany.cn

df -h;  du -sh *
来源：http://vau.pengpengdd.cyou

[R62] 找最占空间的文件
来源：http://own.fzhhl.top

du -ah . | sort -rh | head -10
来源：http://rut.xylfe.cn

[R63] 内存与进程
来源：http://lrw.fzhhl.top

free -h;  ps aux | grep nginx
来源：http://vlm.yj20258888.top

[R64] 结束进程
来源：http://hag.ydjk.org.cn

kill -9 $(pgrep -f app.py)
来源：http://xma.zhiwuduotai.top

[R65] 查看端口占用
来源：http://abq.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wpg.hywenlv.cn

[R66] 定时任务
来源：http://uyi.ywan-chungtsiang.top

crontab -e;  crontab -l
来源：http://ver.hnqzz.top

[R67] 生成随机十六进制串
来源：http://ygy.sweek.top

openssl rand -hex 16
来源：http://svm.zhijiandao.cn

[R68] 计算文件校验值
来源：http://vie.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mgv.cqqwz.cn

[R69] 生成随机密码
来源：http://jak.ivvv.top

head -c 16 /dev/urandom | base64
来源：http://gbh.guannengcc.top

[R70] 时间戳与互转
来源：http://qno.sxryk.cn

date +%s;  date -d @1700000000
来源：http://xbt.bbcook.cn

[R71] 日期格式化
来源：http://was.hysaishi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hfb.mhx1999.top

[R72] 等待端口就绪
来源：http://pga.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://apv.chenzaomai.com

[R73] 分割大日志
来源：http://wfa.fktsv.cn

split -l 1000 big.log part_
来源：http://qlb.jinqigfzy.top

[R74] 批量重命名
来源：http://wif.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pbx.andypj.xyz

[R75] 导出环境变量
来源：http://aim.chenlongwang.top

export PATH="$HOME/bin:$PATH"
来源：http://dbk.havefunace.top

[R76] 使用临时文件
来源：http://znp.9152youxi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nse.sysykeji.top

[R77] 读取用户输入
来源：http://rwu.hnxiangtu.top

read -rp "请输入: " ans
来源：http://fbz.hesvh.cn

[R78] 交互式菜单
来源：http://owp.wangshuangyany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://agb.gzhubu.top

[R79] 解析命令行选项
来源：http://xyh.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://duw.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://ejn.jinyuanbaomall.cn

time ./run.sh
来源：http://ccd.tian-w.cn

================================================================================
来源：http://xeg.snrcjt.cn

S. C / C++ 专题
来源：http://qgq.vehdjk.com

================================================================================
来源：http://lfb.xylfe.cn

[S01] C：Hello World
来源：http://ddl.jinqigfzy.top

#include <stdio.h>
来源：http://pqe.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://jgc.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://jrk.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://gli.vehdjk.com

[S03] C：读入整数
来源：http://wib.haohaochexian.top

int x; scanf("%d", &x);
来源：http://zhw.tianlin.xyz

[S04] C：字符串复制
来源：http://zpw.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://mhc.fktsv.cn

[S05] C：字符串长度
来源：http://eik.cucudq.cn

strlen(s)
来源：http://mhj.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://hpw.yj20258.top

strcmp(a, b) == 0
来源：http://mbv.zhengqikj.top

[S07] C：数组遍历求和
来源：http://qzy.zhixingplan.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nsk.pycfn.com

[S08] C：动态内存分配与释放
来源：http://jmn.xylfe.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xye.zhijiandao.cn

[S09] C：结构体定义与初始化
来源：http://iws.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nvs.yuanzhike.top

[S10] C：指针与解引用
来源：http://wjz.hnqzz.top

int *p = &a;  *p = 5;
来源：http://eef.yfazqb.com

[S11] C：逐行读文件
来源：http://xdq.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://dzf.sysykeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://laf.jlsjyb.cn

fclose(f);
来源：http://rvn.cashguo.top

[S12] C：写文件
来源：http://zic.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://shc.fzhhl.top

[S13] C：宏定义
来源：http://wqy.hfpthk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jwo.xingfuxueyuan.xyz

[S14] C：枚举
来源：http://hgb.epnwcf.com

enum Color { RED, GREEN, BLUE };
来源：http://hsh.jinqigfzy.top

[S15] C：类型转换
来源：http://skt.chenjidiqi.icu

(double) a / b
来源：http://vzk.vqdsnc.cn

[S16] C：位操作置位
来源：http://dry.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://frn.cashguo.top

[S17] C：安全拼接字符串
来源：http://cfs.svipenyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://apv.fzhhl.top

[S18] C：命令行参数
来源：http://wjr.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://kgf.gaohongyu789.top

[S19] C：快速排序
来源：http://khf.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://lll.hfpthk.cn

[S20] C：二分查找
来源：http://gqy.yueranfly.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://byp.andypj.xyz

[S21] C：字符类别判断
来源：http://zud.jinqigfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://evb.shanyushiyangkeji.top

[S22] C：字符串转数字
来源：http://gek.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://xav.dianchejie.cn

[S23] C：随机数
来源：http://iir.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xow.xziqi.cn

[S24] C：获取本地时间
来源：http://cyl.dashuyun.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oio.aibaodan.cn

[S25] C：内存拷贝
来源：http://nib.yj20258888.top

memcpy(dst, src, n);
来源：http://gjz.cqqwz.cn

[S26] C：内存清零
来源：http://hea.shangyingyoupin.top

memset(a, 0, sizeof a);
来源：http://fwg.cashguo.top

[S27] C：定义常量
来源：http://bfk.pengpengdd.cyou

const double PI = 3.14159;
来源：http://yyz.pengpengdd.cyou

[S28] C：静态变量
来源：http://saw.kuanghao11.cn

static int counter = 0;
来源：http://acn.ybcxt.top

[S29] C：变参函数
来源：http://yrs.kuanghao11.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ada.jianghu66.top

[S30] C：头文件保护
来源：http://iar.hfpthk.cn

#ifndef X_H
来源：http://cfc.jlsjyb.cn

#define X_H
来源：http://iox.hesvh.cn

#endif
来源：http://xxg.tian-w.cn

[S31] C++：Hello World
来源：http://qtf.gotoacloud.top

#include <iostream>
来源：http://xqa.ydzc1.top

int main() { std::cout << "Hello\n"; }
来源：http://zin.epnwcf.com

[S32] C++：字符串
来源：http://vay.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://ypx.nwbrower.top

[S33] C++：vector 增删
来源：http://gcg.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bqm.birdmap.top

[S34] C++：遍历 vector
来源：http://txn.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://bwe.sjlbkw.cn

[S35] C++：map
来源：http://mnh.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dyb.sufxvd.cn

[S36] C++：unordered_map
来源：http://ngh.gaohongyu789.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hjw.hfpthk.cn

[S37] C++：set
来源：http://lvu.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fia.wangshuangyany.cn

[S38] C++：排序
来源：http://umn.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://zps.jqgufenzy.top


<!-- 参考信息 -->