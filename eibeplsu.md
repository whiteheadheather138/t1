代发 wailian999

ANALYZE TABLE users;
来源：http://tjz.havefunace.top

[Q71] 查看建表语句
来源：http://lhw.birdmap.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wqn.ybcxt.top

[Q72] 查看索引
来源：http://uxa.tarul.cn

SHOW INDEX FROM users;
来源：http://nhg.yj20258.top

[Q73] 查看表状态
来源：http://qoc.epnwcf.com

SHOW TABLE STATUS LIKE 'users';
来源：http://ufe.gzhubu.top

[Q74] 强制使用索引
来源：http://zce.yuanzhike.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kas.fengsongda.top

[Q75] 日期格式化
来源：http://oaz.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rxq.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ult.ybcxt.top

[Q76] 按天统计
来源：http://fzd.hcnkem.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pqj.bjfxy.top

[Q77] 时间加减
来源：http://yai.c1oappe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ejn.redwolf501.top

[Q78] 当前时间
来源：http://tfm.sufxvd.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dal.zhoulong.xyz

[Q79] 字符串拼接
来源：http://yyh.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bbn.tianlin.xyz

[Q80] 字符串截取
来源：http://tdc.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nqt.0kj1m.cn

[Q81] 字符串替换
来源：http://mex.birdmap.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vyp.gaohongyu789.top

[Q82] 字符长度与字节长度
来源：http://mym.hfpthk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qfd.svipenyu.cn

[Q83] 大小写转换
来源：http://whe.tianlin.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lcu.shangyingyoupin.top

[Q84] 去除首尾空格
来源：http://cnx.chenlongwang.top

SELECT TRIM(name) FROM users;
来源：http://meb.jqgufenzy.top

[Q85] 数值取整
来源：http://hms.jinghuilouyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jdx.hammf.cn

[Q86] 读取 JSON 字段
来源：http://qsh.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jnb.hnxiangtu.top

[Q87] JSON 字段做条件
来源：http://rfk.snrcjt.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://syv.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://ghn.xuanzx.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qot.hesvh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ugu.jinqigufen.top

[Q89] 判断表是否存在
来源：http://mda.sjlbkw.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gck.quarkkingdee.top

[Q90] 生成序号列
来源：http://qcw.uphjek.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hdh.fktsv.cn

================================================================================
来源：http://goo.mhx1999.top

R. Bash 专题
来源：http://cjf.sufxvd.cn

================================================================================
来源：http://oxp.hongshengwenyu.top

[R01] shebang 与严格模式
来源：http://tqa.ctjpmb.com

#!/usr/bin/env bash
来源：http://wtb.havefunace.top

set -euo pipefail
来源：http://bfh.haohaochexian.top

[R02] 变量赋值与使用
来源：http://nrs.sufxvd.cn

name="Tom"; echo "$name"
来源：http://qgw.gogol.net.cn

[R03] 只读变量
来源：http://jjo.fanxiaobao.xyz

readonly PI=3.14
来源：http://xfa.aibaodan.cn

[R04] 位置参数
来源：http://ild.smart0.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kvf.zhoulong.xyz

[R05] 参数默认值
来源：http://yrz.yongpay.top

name="${1:-default}"
来源：http://oly.hammf.cn

[R06] 判断命令是否存在
来源：http://wox.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://epz.nwbrower.top

[R07] if 判断文件
来源：http://cwo.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rdv.daxiang520.top

[R08] 数值比较
来源：http://kvl.jinyuanbaomall.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kja.fehbvm.com

[R09] 字符串比较
来源：http://dgq.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rem.aizwys.cn

[R10] 正则匹配
来源：http://fty.daxiang520.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://itm.ivvv.top

[R11] case 多分支
来源：http://mlo.cheryme.top

case "$1" in
来源：http://wud.guannengcc.top

start) echo "启动" ;;
来源：http://gcu.snrcjt.cn

stop)  echo "停止" ;;
来源：http://irx.meibo888.top

*)     echo "未知命令" ;;
来源：http://brz.ehwqpu.com

esac
来源：http://pdi.bbcook.cn

[R12] for 遍历文件
来源：http://pxe.sjlbkw.cn

for f in *.txt; do echo "$f"; done
来源：http://xxh.cdnleiting.top

[R13] for 计数循环
来源：http://cdc.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://cpz.zhiwuduotai.top

[R14] C 风格 for
来源：http://och.fanxiaobao.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lle.ybcxt.top

[R15] while 逐行读文件
来源：http://lpe.fanxiaobao.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ezm.jinqigufen.top

[R16] until 等待条件
来源：http://wir.daria6918.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ste.zhijiandao.cn

[R17] 数组定义与取值
来源：http://sqi.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://gzr.daxiang520.top

[R18] 遍历数组
来源：http://zkx.hcnkem.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vnx.birdmap.top

[R19] 数组长度
来源：http://umc.gogol.net.cn

echo "${#arr[@]}"
来源：http://afi.jqgfzy.top

[R20] 关联数组（字典）
来源：http://cbm.nwbrower.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uvb.kuanghao11.cn

[R21] 字符串长度
来源：http://dkv.chenlongwang.top

echo "${#s}"
来源：http://ipy.guannengcc.top

[R22] 截取子串
来源：http://jwd.cheryme.top

echo "${s:0:5}"
来源：http://abt.xziqi.cn

[R23] 字符串替换
来源：http://kig.wangshuangyany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eok.chenzaomai.com

[R24] 大小写转换
来源：http://hka.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cjx.ehwqpu.com

[R25] 去后缀 / 去前缀
来源：http://jam.jqgfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gib.jqgufenzy.top

[R26] 命令替换
来源：http://fja.bbcook.cn

now=$(date +%F); echo "$now"
来源：http://xbb.xuetiantiany.cn

[R27] 算术展开
来源：http://yhw.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://gio.wangshuangyany.cn

[R28] 浮点运算
来源：http://huo.sweek.top

echo "scale=2; 10/3" | bc
来源：http://tpg.zdqjudy.top

[R29] 定义函数
来源：http://mkf.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eep.yangfankeji.com

[R30] 函数返回状态码
来源：http://iqd.tarul.cn

f() { return 0; }; f || echo "失败了"
来源：http://kya.cheryme.top

[R31] 局部变量
来源：http://itu.xziqi.cn

f() { local x=1; echo "$x"; }
来源：http://xnh.sweek.top

[R32] 参数个数校验
来源：http://anm.ywan-chungtsiang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sgq.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://lnp.ctjpmb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://shv.ydzc1.top

[R34] 退出时清理
来源：http://tcr.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://qsq.yonumen.top

[R35] 后台执行并等待
来源：http://ktj.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://rhd.ivvv.top

[R36] 并发执行多个任务
来源：http://ixt.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qvr.ctjpmb.com

[R37] 把输出赋给变量
来源：http://xkh.snrcjt.cn

files=$(ls -1)
来源：http://fzo.hammf.cn

[R38] 管道串联
来源：http://kwn.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://avv.snrcjt.cn

[R39] 重定向标准输出与错误
来源：http://gbk.xinyue.icu

cmd > out.log 2>&1
来源：http://txr.uphjek.com

[R40] 追加写日志
来源：http://olc.jinghuilouyu.cn

echo "log" >> out.log
来源：http://yqb.sjlbkw.cn

[R41] 丢弃输出
来源：http://uxr.epnwcf.com

cmd >/dev/null 2>&1
来源：http://src.fzhhl.top

[R42] 输入重定向
来源：http://bzv.chenjidiqi.icu

wc -l < a.txt
来源：http://mpw.zdqjudy.top

[R43] 按名字查找文件
来源：http://pid.zhongyouzk.top

find . -name "*.log" -type f
来源：http://szw.ctjpmb.com

[R44] 按修改时间查找
来源：http://ssv.fehbvm.com

find . -mtime -7 -type f
来源：http://crp.yangfankeji.com

[R45] 批量删除
来源：http://cus.xuanzx.com

find . -name "*.tmp" -delete
来源：http://slj.yfazqb.com

[R46] 递归替换文件内容
来源：http://kdj.jinghuilouyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vbs.mhx1999.top

[R47] sed 单行替换
来源：http://apt.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://vdu.zhiwuduotai.top

[R48] awk 取指定列
来源：http://klf.birdmap.top

awk '{print $1, $3}' a.txt
来源：http://zjm.nwbrower.top

[R49] awk 带条件
来源：http://pea.pengpengdd.cyou

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://afi.yonumen.top

[R50] awk 求和
来源：http://vsy.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qrs.jqgfzy.top

[R51] 排序去重取前几
来源：http://cni.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://hzr.sxryk.cn

[R52] 统计行数
来源：http://efj.mhx1999.top

wc -l a.txt
来源：http://lhf.xuanzx.com

[R53] 查看文件头与实时尾
来源：http://yau.sxryk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wfa.ydjk.org.cn

[R54] 比较两个文件
来源：http://xlz.zhixingplan.top

diff a.txt b.txt
来源：http://skz.vqdsnc.cn

[R55] 压缩与解压
来源：http://alh.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dln.hcnkem.com

[R56] 远程拷贝
来源：http://ngu.chenjidiqi.icu

scp file user@host:/path/
来源：http://dqh.9152youxi.cn

[R57] 远程执行命令
来源：http://ysy.dashuyun.cn

ssh user@host 'uptime'
来源：http://hht.ybcxt.top

[R58] 下载文件
来源：http://wko.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zwu.andypj.xyz

[R59] 发 POST JSON
来源：http://hlu.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pxf.feifeiyinyue.top

[R60] 只看 HTTP 状态码
来源：http://mtl.sufxvd.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://msi.ybcxt.top

[R61] 磁盘占用
来源：http://gkv.hywenlv.cn

df -h;  du -sh *
来源：http://awe.vehdjk.com

[R62] 找最占空间的文件
来源：http://twp.cheryme.top

du -ah . | sort -rh | head -10
来源：http://sli.pycfn.com

[R63] 内存与进程
来源：http://que.jiagoushi.top

free -h;  ps aux | grep nginx
来源：http://iiu.guowangkeji.top

[R64] 结束进程
来源：http://phk.guowangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://ihi.epnwcf.com

[R65] 查看端口占用
来源：http://wlt.jyoumei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kug.tanke756.top

[R66] 定时任务
来源：http://yje.hfpthk.cn

crontab -e;  crontab -l
来源：http://wrs.gogol.net.cn

[R67] 生成随机十六进制串
来源：http://yuj.tarul.cn

openssl rand -hex 16
来源：http://nsi.cheryme.top

[R68] 计算文件校验值
来源：http://dvr.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://frr.aizwys.cn

[R69] 生成随机密码
来源：http://xjc.xingfuxueyuan.xyz

head -c 16 /dev/urandom | base64
来源：http://fgd.quarkkingdee.top

[R70] 时间戳与互转
来源：http://crp.yangfankeji.com

date +%s;  date -d @1700000000
来源：http://mgn.aibaodan.cn

[R71] 日期格式化
来源：http://xji.fktsv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gwo.sweek.top

[R72] 等待端口就绪
来源：http://vzn.shanyushiyangtech.top

until nc -z localhost 3306; do sleep 1; done
来源：http://axg.cdnleiting.top

[R73] 分割大日志
来源：http://spk.hfpthk.cn

split -l 1000 big.log part_
来源：http://yci.xylfe.cn

[R74] 批量重命名
来源：http://lwk.xuetiantiany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://etd.fktsv.cn

[R75] 导出环境变量
来源：http://xsw.vehdjk.com

export PATH="$HOME/bin:$PATH"
来源：http://hgp.hnqzz.top

[R76] 使用临时文件
来源：http://dye.zhaomingkeji.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wuw.zhengqikj.top

[R77] 读取用户输入
来源：http://udq.chenlongwang.top

read -rp "请输入: " ans
来源：http://eof.cdnleiting.top

[R78] 交互式菜单
来源：http://aql.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qsv.zhaomingkeji.xyz

[R79] 解析命令行选项
来源：http://lby.yj202588.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aan.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://liz.sjlbkw.cn

time ./run.sh
来源：http://lrg.cheryme.top

================================================================================
来源：http://efi.yangfankeji.com

S. C / C++ 专题
来源：http://kmc.fehbvm.com

================================================================================
来源：http://piu.ydjk.org.cn

[S01] C：Hello World
来源：http://ugk.fanxiaobao.xyz

#include <stdio.h>
来源：http://yjm.guowangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bjq.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://ffs.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://ixs.ctjpmb.com

[S03] C：读入整数
来源：http://iaw.zhoulong.xyz

int x; scanf("%d", &x);
来源：http://ndh.redwolf501.top

[S04] C：字符串复制
来源：http://xby.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://tdc.chenzaomai.com

[S05] C：字符串长度
来源：http://mnv.haohaochexian.top

strlen(s)
来源：http://wtf.svipenyu.cn

[S06] C：字符串比较
来源：http://sng.zhengqikj.top

strcmp(a, b) == 0
来源：http://nqc.guowangkeji.top

[S07] C：数组遍历求和
来源：http://lyi.nanxuanxn.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xlq.shanyushiyangtech.top

[S08] C：动态内存分配与释放
来源：http://iso.xylfe.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wkg.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://mrr.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pmv.yvedp.cn

[S10] C：指针与解引用
来源：http://hqn.sufxvd.cn

int *p = &a;  *p = 5;
来源：http://iwx.ctjpmb.com

[S11] C：逐行读文件
来源：http://tob.quarkkingdee.top

FILE *f = fopen("a.txt", "r");
来源：http://cvy.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pgu.tarul.cn

fclose(f);
来源：http://iqa.redwolf501.top

[S12] C：写文件
来源：http://ihy.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nyv.ppjwa.cn

[S13] C：宏定义
来源：http://ngi.yuxming.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vql.gogol.net.cn

[S14] C：枚举
来源：http://vfw.9152youxi.cn

enum Color { RED, GREEN, BLUE };
来源：http://omy.ppjwa.cn

[S15] C：类型转换
来源：http://mqt.c1oappe.top

(double) a / b
来源：http://mxc.zdbjq.cn

[S16] C：位操作置位
来源：http://qsf.zhoulong.xyz

x |= (1 << 3);
来源：http://gyc.zhengqikj.top

[S17] C：安全拼接字符串
来源：http://fzf.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mwu.kuanghao11.cn

[S18] C：命令行参数
来源：http://wrc.yvedp.cn

int main(int argc, char **argv)
来源：http://xym.hnxiangtu.top

[S19] C：快速排序
来源：http://wql.cheryme.top

qsort(a, n, sizeof(int), cmp);
来源：http://aiu.uphjek.com

[S20] C：二分查找
来源：http://dpq.tarul.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qpl.yangfankeji.com

[S21] C：字符类别判断
来源：http://oqt.fengsongda.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xfn.chenlongwang.top

[S22] C：字符串转数字
来源：http://pwk.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://uia.jqgufenzy.top

[S23] C：随机数
来源：http://ofi.cdnleiting.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mvz.guannengcc.top

[S24] C：获取本地时间
来源：http://tnv.yueranfly.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qhe.svipenyu.cn

[S25] C：内存拷贝
来源：http://kni.zdqjudy.top

memcpy(dst, src, n);
来源：http://skp.shzxlz.cn

[S26] C：内存清零
来源：http://tfh.chenzaomai.com

memset(a, 0, sizeof a);
来源：http://bxy.ctjpmb.com

[S27] C：定义常量
来源：http://llr.ppjwa.cn

const double PI = 3.14159;
来源：http://teu.sufxvd.cn

[S28] C：静态变量
来源：http://ocz.jinyuanbaomall.cn

static int counter = 0;
来源：http://uto.cucudq.cn

[S29] C：变参函数
来源：http://udb.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hve.shuidangran.top

[S30] C：头文件保护
来源：http://bdu.jinyuanbaomall.cn

#ifndef X_H
来源：http://tnq.fktsv.cn

#define X_H
来源：http://omf.yonumen.top

#endif
来源：http://plc.daria6918.cn

[S31] C++：Hello World
来源：http://jng.mhx1999.top

#include <iostream>
来源：http://rmq.yuanzhike.top

int main() { std::cout << "Hello\n"; }
来源：http://pdj.birdmap.top

[S32] C++：字符串
来源：http://vrp.xuetiantiany.cn

std::string s = "hi";  s += "!";
来源：http://ijv.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://rum.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dzj.316326.xyz

[S34] C++：遍历 vector
来源：http://ibm.shanyushiyangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://kqo.mhx1999.top

[S35] C++：map
来源：http://asg.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wqx.fehbvm.com

[S36] C++：unordered_map
来源：http://mpm.shanyushiyangtech.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://toe.dashuyun.cn

[S37] C++：set
来源：http://mhl.nanxinkj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://met.epnwcf.com

[S38] C++：排序
来源：http://rlx.ppjwa.cn

std::sort(v.begin(), v.end());
来源：http://ufk.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://hbc.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hou.tarul.cn

[S40] C++：查找元素
来源：http://uqp.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://caa.ivvv.top


<!-- 参考信息 -->