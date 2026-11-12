代发 wailian999

SHOW INDEX FROM users;
来源：http://uzn.birdmap.top

[Q73] 查看表状态
来源：http://qxa.hnqzz.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jqg.haohaochexian.top

[Q74] 强制使用索引
来源：http://tgy.zhongyouzk.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://trh.shanyushiyangtech.top

[Q75] 日期格式化
来源：http://kat.kuanghao11.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gzx.pengpengdd.cyou

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rol.tianlin.xyz

[Q76] 按天统计
来源：http://waq.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nxs.ybcxt.top

[Q77] 时间加减
来源：http://sjq.sjlbkw.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gml.yj202588.top

[Q78] 当前时间
来源：http://bhy.yj20258888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yxw.birdmap.top

[Q79] 字符串拼接
来源：http://rlm.birdmap.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iak.xziqi.cn

[Q80] 字符串截取
来源：http://jlx.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qby.gotoacloud.top

[Q81] 字符串替换
来源：http://qni.uphjek.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rey.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://ayn.shanyushiyangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gkb.yuxming.cn

[Q83] 大小写转换
来源：http://zlk.iojbl.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ibk.xziqi.cn

[Q84] 去除首尾空格
来源：http://zhc.iojbl.cn

SELECT TRIM(name) FROM users;
来源：http://wcz.mhx1999.top

[Q85] 数值取整
来源：http://awx.9152youxi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qpz.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://ard.meibo888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pvs.yuanzhike.top

[Q87] JSON 字段做条件
来源：http://tei.jiagoushi.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zhq.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://ghy.fengsongda.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wqx.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xqk.nanxinkj.top

[Q89] 判断表是否存在
来源：http://zcv.tian-w.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xmp.tianlin.xyz

[Q90] 生成序号列
来源：http://akt.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://flj.wangdashe.top

================================================================================
来源：http://zpa.sysykeji.top

R. Bash 专题
来源：http://qir.zhongyouzk.top

================================================================================
来源：http://jgs.yonumen.top

[R01] shebang 与严格模式
来源：http://wsg.smart0.xyz

#!/usr/bin/env bash
来源：http://buy.shanyushiyangtech.top

set -euo pipefail
来源：http://jrw.jinqigufen.top

[R02] 变量赋值与使用
来源：http://kcc.tianlin.xyz

name="Tom"; echo "$name"
来源：http://jma.c1oappe.top

[R03] 只读变量
来源：http://usi.gaohongyu789.top

readonly PI=3.14
来源：http://lpq.tianlin.xyz

[R04] 位置参数
来源：http://zok.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://skn.gotoacloud.top

[R05] 参数默认值
来源：http://xod.yvedp.cn

name="${1:-default}"
来源：http://kdk.yj20258.top

[R06] 判断命令是否存在
来源：http://jgu.redwolf501.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aqc.316326.xyz

[R07] if 判断文件
来源：http://beh.redwolf501.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://byz.nwbrower.top

[R08] 数值比较
来源：http://yua.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://jgo.aizwys.cn

[R09] 字符串比较
来源：http://tny.ivvv.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dep.316326.xyz

[R10] 正则匹配
来源：http://sph.zhiwuduotai.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zwk.sysykeji.top

[R11] case 多分支
来源：http://pbd.guowangkeji.top

case "$1" in
来源：http://wjl.xylfe.cn

start) echo "启动" ;;
来源：http://dvr.jinqigfzy.top

stop)  echo "停止" ;;
来源：http://oyg.jinyuanbaomall.cn

*)     echo "未知命令" ;;
来源：http://ajg.yangfankeji.com

esac
来源：http://bxv.hywenlv.cn

[R12] for 遍历文件
来源：http://ipg.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://unj.zhongyouzk.top

[R13] for 计数循环
来源：http://dsk.jinyuanbaomall.cn

for i in {1..10}; do echo "$i"; done
来源：http://uul.yongpay.top

[R14] C 风格 for
来源：http://plv.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ylk.guowangkeji.top

[R15] while 逐行读文件
来源：http://fti.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iwk.shangyingyoupin.top

[R16] until 等待条件
来源：http://lwf.hcnkem.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gdw.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://lfc.zhijiandao.cn

arr=(a b c); echo "${arr[0]}"
来源：http://evl.yongpay.top

[R18] 遍历数组
来源：http://nja.hfpthk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tub.pycfn.com

[R19] 数组长度
来源：http://opy.hnxiangtu.top

echo "${#arr[@]}"
来源：http://vsx.iojbl.cn

[R20] 关联数组（字典）
来源：http://hwb.jlsjyb.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://agq.hcnkem.com

[R21] 字符串长度
来源：http://ruu.ivvv.top

echo "${#s}"
来源：http://gjw.chenlongwang.top

[R22] 截取子串
来源：http://yga.jyoumei.cn

echo "${s:0:5}"
来源：http://oka.zhongyouzk.top

[R23] 字符串替换
来源：http://kis.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wov.sweek.top

[R24] 大小写转换
来源：http://eux.sysykeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://tar.uphjek.com

[R25] 去后缀 / 去前缀
来源：http://vsl.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zbj.haohaochexian.top

[R26] 命令替换
来源：http://uec.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://kha.kuanghao11.cn

[R27] 算术展开
来源：http://ggc.feifeiyinyue.top

echo $((1 + 2 * 3))
来源：http://tkj.tanke756.top

[R28] 浮点运算
来源：http://dkh.chenzaomai.com

echo "scale=2; 10/3" | bc
来源：http://tkc.cheryme.top

[R29] 定义函数
来源：http://kbc.jianghu66.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://scv.zhiwuduotai.top

[R30] 函数返回状态码
来源：http://dfy.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://whr.ywan-chungtsiang.top

[R31] 局部变量
来源：http://pwm.daxiang520.top

f() { local x=1; echo "$x"; }
来源：http://lpp.ydjk.org.cn

[R32] 参数个数校验
来源：http://qwi.xinyue.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lsr.shangyingyoupin.top

[R33] 捕获错误并提示行号
来源：http://pln.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iyd.jiagoushi.top

[R34] 退出时清理
来源：http://jak.sweek.top

trap 'rm -f "$tmp"' EXIT
来源：http://pxr.xuanzx.com

[R35] 后台执行并等待
来源：http://zam.hammf.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xqo.svipenyu.cn

[R36] 并发执行多个任务
来源：http://kgr.svipenyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wys.zdqjudy.top

[R37] 把输出赋给变量
来源：http://brb.ydjk.org.cn

files=$(ls -1)
来源：http://sco.kuanghao11.cn

[R38] 管道串联
来源：http://jvp.fanxiaobao.xyz

cat a.txt | grep -i error | wc -l
来源：http://brr.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://ocz.quarkkingdee.top

cmd > out.log 2>&1
来源：http://owy.vqdsnc.cn

[R40] 追加写日志
来源：http://mhg.aizwys.cn

echo "log" >> out.log
来源：http://ggo.yonumen.top

[R41] 丢弃输出
来源：http://bom.ehwqpu.com

cmd >/dev/null 2>&1
来源：http://bzx.dashuyun.cn

[R42] 输入重定向
来源：http://uhr.ctjpmb.com

wc -l < a.txt
来源：http://rhf.gotoacloud.top

[R43] 按名字查找文件
来源：http://gbh.xinyue.icu

find . -name "*.log" -type f
来源：http://qgy.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://xqi.guowangkeji.top

find . -mtime -7 -type f
来源：http://oaz.guannengcc.top

[R45] 批量删除
来源：http://uat.andypj.xyz

find . -name "*.tmp" -delete
来源：http://gcn.xuetiantiany.cn

[R46] 递归替换文件内容
来源：http://xif.sweek.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qpa.daria6918.cn

[R47] sed 单行替换
来源：http://tlv.nwbrower.top

sed -i 's/foo/bar/g' a.txt
来源：http://vjc.zdbjq.cn

[R48] awk 取指定列
来源：http://owe.daxiang520.top

awk '{print $1, $3}' a.txt
来源：http://qby.fktsv.cn

[R49] awk 带条件
来源：http://ghz.pengpengdd.cyou

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zwk.daria6918.cn

[R50] awk 求和
来源：http://wch.yonumen.top

awk '{s += $2} END {print s}' a.txt
来源：http://yuz.cashguo.top

[R51] 排序去重取前几
来源：http://jlc.zhiwuduotai.top

sort a.txt | uniq -c | sort -rn | head
来源：http://czh.zhoulong.xyz

[R52] 统计行数
来源：http://zis.yj202588.top

wc -l a.txt
来源：http://ucp.zdqjudy.top

[R53] 查看文件头与实时尾
来源：http://xwm.c1oappe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://diz.wangdashe.top

[R54] 比较两个文件
来源：http://txs.zhaomingkeji.xyz

diff a.txt b.txt
来源：http://ifw.gogol.net.cn

[R55] 压缩与解压
来源：http://ftn.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jzd.jqgfzy.top

[R56] 远程拷贝
来源：http://yzq.ivvv.top

scp file user@host:/path/
来源：http://eqo.iojbl.cn

[R57] 远程执行命令
来源：http://xif.gaohongyu789.top

ssh user@host 'uptime'
来源：http://vii.gaohongyu789.top

[R58] 下载文件
来源：http://trt.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mpk.hywenlv.cn

[R59] 发 POST JSON
来源：http://owx.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yqn.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://pnk.hnqzz.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kln.guowangkeji.top

[R61] 磁盘占用
来源：http://auh.cheryme.top

df -h;  du -sh *
来源：http://pvm.epnwcf.com

[R62] 找最占空间的文件
来源：http://xaw.birdmap.top

du -ah . | sort -rh | head -10
来源：http://idy.9152youxi.cn

[R63] 内存与进程
来源：http://xaj.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://hap.iojbl.cn

[R64] 结束进程
来源：http://ilz.daria6918.cn

kill -9 $(pgrep -f app.py)
来源：http://jro.aizwys.cn

[R65] 查看端口占用
来源：http://usr.cqqwz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vtu.pengpengdd.cyou

[R66] 定时任务
来源：http://gmo.fengsongda.top

crontab -e;  crontab -l
来源：http://icr.zhiwuduotai.top

[R67] 生成随机十六进制串
来源：http://deq.hesvh.cn

openssl rand -hex 16
来源：http://kps.guannengcc.top

[R68] 计算文件校验值
来源：http://kkv.zhongyouzk.top

sha256sum a.txt;  md5sum a.txt
来源：http://grb.ppjwa.cn

[R69] 生成随机密码
来源：http://pfx.cashguo.top

head -c 16 /dev/urandom | base64
来源：http://vio.dianchejie.cn

[R70] 时间戳与互转
来源：http://ium.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://bju.zycfv.cn

[R71] 日期格式化
来源：http://ujo.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eml.shuidangran.top

[R72] 等待端口就绪
来源：http://bns.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fii.316326.xyz

[R73] 分割大日志
来源：http://qdo.ivvv.top

split -l 1000 big.log part_
来源：http://ttu.dianchejie.cn

[R74] 批量重命名
来源：http://xzh.uphjek.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://byx.316326.xyz

[R75] 导出环境变量
来源：http://ggm.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://kya.tianlin.xyz

[R76] 使用临时文件
来源：http://dra.epnwcf.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lpb.guowangkeji.top

[R77] 读取用户输入
来源：http://jum.epnwcf.com

read -rp "请输入: " ans
来源：http://ugf.hammf.cn

[R78] 交互式菜单
来源：http://yok.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vei.jinghuilouyu.cn

[R79] 解析命令行选项
来源：http://evh.hammf.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pks.c1oappe.top

[R80] 查看脚本执行耗时
来源：http://qqu.yuanzhike.top

time ./run.sh
来源：http://sht.jqgufenzy.top

================================================================================
来源：http://jvd.cucudq.cn

S. C / C++ 专题
来源：http://xjp.jqgufenzy.top

================================================================================
来源：http://joe.jinyuanbaomall.cn

[S01] C：Hello World
来源：http://fwm.yj202588.top

#include <stdio.h>
来源：http://nus.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lds.zhixingplan.top

[S02] C：变量与格式化输出
来源：http://aon.hesvh.cn

int a = 10; printf("%d\n", a);
来源：http://tpm.xuanzx.com

[S03] C：读入整数
来源：http://cbf.xingfuxueyuan.xyz

int x; scanf("%d", &x);
来源：http://pat.quarkkingdee.top

[S04] C：字符串复制
来源：http://seh.zhongyouzk.top

char dst[32]; strcpy(dst, "hi");
来源：http://vup.hammf.cn

[S05] C：字符串长度
来源：http://xey.snrcjt.cn

strlen(s)
来源：http://ijo.shzxlz.cn

[S06] C：字符串比较
来源：http://ijx.zhongyouzk.top

strcmp(a, b) == 0
来源：http://fuk.pycfn.com

[S07] C：数组遍历求和
来源：http://cny.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://phl.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://bnq.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gdk.ppjwa.cn

[S09] C：结构体定义与初始化
来源：http://yxz.yuxming.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bad.yongpay.top

[S10] C：指针与解引用
来源：http://luz.quarkkingdee.top

int *p = &a;  *p = 5;
来源：http://qov.guannengcc.top

[S11] C：逐行读文件
来源：http://kox.jianghu66.top

FILE *f = fopen("a.txt", "r");
来源：http://yhh.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fnh.chenzaomai.com

fclose(f);
来源：http://azt.zhiwuduotai.top

[S12] C：写文件
来源：http://yzt.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xmg.aibaodan.cn

[S13] C：宏定义
来源：http://ntw.xziqi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rhz.kuanghao11.cn

[S14] C：枚举
来源：http://pcw.shuidangran.top

enum Color { RED, GREEN, BLUE };
来源：http://smw.daxiang520.top

[S15] C：类型转换
来源：http://bve.xylfe.cn

(double) a / b
来源：http://elz.ybcxt.top

[S16] C：位操作置位
来源：http://gim.yongpay.top

x |= (1 << 3);
来源：http://zro.jinyuanbaomall.cn

[S17] C：安全拼接字符串
来源：http://bib.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hdg.cashguo.top

[S18] C：命令行参数
来源：http://umm.pycfn.com

int main(int argc, char **argv)
来源：http://vup.feifeiyinyue.top

[S19] C：快速排序
来源：http://wpf.yuxming.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iwy.quarkkingdee.top

[S20] C：二分查找
来源：http://zvw.quarkkingdee.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://asl.cucudq.cn

[S21] C：字符类别判断
来源：http://nfo.yfazqb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gxq.yfazqb.com

[S22] C：字符串转数字
来源：http://ukn.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://xdy.quarkkingdee.top

[S23] C：随机数
来源：http://fjh.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ofz.dashuyun.cn

[S24] C：获取本地时间
来源：http://cco.pengpengdd.cyou

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oyv.ydjk.org.cn

[S25] C：内存拷贝
来源：http://eru.yj20258888.top

memcpy(dst, src, n);
来源：http://ynx.ivvv.top

[S26] C：内存清零
来源：http://qgn.fengsongda.top

memset(a, 0, sizeof a);
来源：http://wtb.sysykeji.top

[S27] C：定义常量
来源：http://twm.feifeiyinyue.top

const double PI = 3.14159;
来源：http://ltg.sufxvd.cn

[S28] C：静态变量
来源：http://ejc.yvedp.cn

static int counter = 0;
来源：http://wtv.jqgfzy.top

[S29] C：变参函数
来源：http://awo.ydzc1.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tpv.xuanzx.com

[S30] C：头文件保护
来源：http://xwv.pycfn.com

#ifndef X_H
来源：http://iev.sxryk.cn

#define X_H
来源：http://ppi.52xcode.cn

#endif
来源：http://omr.smart0.xyz

[S31] C++：Hello World
来源：http://kcl.redwolf501.top

#include <iostream>
来源：http://jzs.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://zue.shanyushiyangtech.top

[S32] C++：字符串
来源：http://riz.cashguo.top

std::string s = "hi";  s += "!";
来源：http://iur.zhengqikj.top

[S33] C++：vector 增删
来源：http://rpg.cucudq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bbi.fanxiaobao.xyz

[S34] C++：遍历 vector
来源：http://zod.jinqigufen.top

for (auto &x : v) { std::cout << x; }
来源：http://dyq.jinghuilouyu.cn

[S35] C++：map
来源：http://zxi.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pmg.guannengcc.top

[S36] C++：unordered_map
来源：http://yqd.yonumen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sdu.wangdashe.top

[S37] C++：set
来源：http://fgl.hesvh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eet.chenzaomai.com

[S38] C++：排序
来源：http://opa.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://lry.yangfankeji.com

[S39] C++：自定义比较器排序
来源：http://nfw.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ote.hongshengwenyu.top

[S40] C++：查找元素
来源：http://lch.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ipf.cqqwz.cn

[S41] C++：类与构造函数
来源：http://ucs.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kch.fktsv.cn

[S42] C++：继承与虚函数
来源：http://hal.yvedp.cn

class B : public Base { public: void f() override {} };
来源：http://vnc.jinghuilouyu.cn


<!-- 参考信息 -->