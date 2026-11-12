代发 wailian999

[Q67] 设置隔离级别
来源：http://mts.zhoulong.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fxc.sufxvd.cn

[Q68] 保存点
来源：http://awl.yongpay.top

SAVEPOINT sp1;
来源：http://kys.fengsongda.top

ROLLBACK TO sp1;
来源：http://eee.shuidangran.top

[Q69] 查看执行计划
来源：http://pby.daxiang520.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://moz.gotoacloud.top

[Q70] 更新统计信息
来源：http://gkq.ybcxt.top

ANALYZE TABLE users;
来源：http://oae.svipenyu.cn

[Q71] 查看建表语句
来源：http://ygb.hesvh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nqe.jinyuanbaomall.cn

[Q72] 查看索引
来源：http://gnx.sxryk.cn

SHOW INDEX FROM users;
来源：http://xly.hesvh.cn

[Q73] 查看表状态
来源：http://fpn.yonumen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wdp.shuidangran.top

[Q74] 强制使用索引
来源：http://qfa.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fys.316326.xyz

[Q75] 日期格式化
来源：http://txn.vqdsnc.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ffo.yuanzhike.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://txs.chenjidiqi.icu

[Q76] 按天统计
来源：http://npu.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://unk.xingfuxueyuan.xyz

[Q77] 时间加减
来源：http://oxi.yuanzhike.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zhe.fzhhl.top

[Q78] 当前时间
来源：http://gvd.9152youxi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dwk.aizwys.cn

[Q79] 字符串拼接
来源：http://ffi.sweek.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://has.hysaishi.cn

[Q80] 字符串截取
来源：http://znm.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kon.yongpay.top

[Q81] 字符串替换
来源：http://ffe.9152youxi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cjs.wangshuangyany.cn

[Q82] 字符长度与字节长度
来源：http://dls.meibo888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://exi.bjfxy.top

[Q83] 大小写转换
来源：http://dvq.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jmd.zycfv.cn

[Q84] 去除首尾空格
来源：http://wih.fktsv.cn

SELECT TRIM(name) FROM users;
来源：http://zqm.redwolf501.top

[Q85] 数值取整
来源：http://gym.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qrd.chenjidiqi.icu

[Q86] 读取 JSON 字段
来源：http://bfd.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mhd.yongpay.top

[Q87] JSON 字段做条件
来源：http://qkv.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rjf.sysykeji.top

[Q88] 行转列（条件聚合）
来源：http://jgr.0kj1m.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tfg.yj20258888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wkn.birdmap.top

[Q89] 判断表是否存在
来源：http://wiq.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rne.hnxiangtu.top

[Q90] 生成序号列
来源：http://fxm.bjfxy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://imp.jqgfzy.top

================================================================================
来源：http://gou.zycfv.cn

R. Bash 专题
来源：http://yrc.yonumen.top

================================================================================
来源：http://nnd.pycfn.com

[R01] shebang 与严格模式
来源：http://htw.cucudq.cn

#!/usr/bin/env bash
来源：http://vez.cqqwz.cn

set -euo pipefail
来源：http://sgw.vehdjk.com

[R02] 变量赋值与使用
来源：http://rss.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://dlg.pengpengdd.cyou

[R03] 只读变量
来源：http://dnv.shzxlz.cn

readonly PI=3.14
来源：http://ita.zhiwuduotai.top

[R04] 位置参数
来源：http://sjw.aibaodan.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yto.redwolf501.top

[R05] 参数默认值
来源：http://cfc.ybcxt.top

name="${1:-default}"
来源：http://niv.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://dcp.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ihs.0kj1m.cn

[R07] if 判断文件
来源：http://xqt.zdbjq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jop.tarul.cn

[R08] 数值比较
来源：http://bgd.zhijiandao.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://khj.havefunace.top

[R09] 字符串比较
来源：http://yha.sxryk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kif.havefunace.top

[R10] 正则匹配
来源：http://vsm.cucudq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tmh.xinyue.icu

[R11] case 多分支
来源：http://bic.52xcode.cn

case "$1" in
来源：http://tzo.jqgufenzy.top

start) echo "启动" ;;
来源：http://ztz.zdbjq.cn

stop)  echo "停止" ;;
来源：http://xmz.jyoumei.cn

*)     echo "未知命令" ;;
来源：http://dwr.xuetiantiany.cn

esac
来源：http://oec.tarul.cn

[R12] for 遍历文件
来源：http://oik.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://vir.jinqigufen.top

[R13] for 计数循环
来源：http://fly.hywenlv.cn

for i in {1..10}; do echo "$i"; done
来源：http://vbn.sysykeji.top

[R14] C 风格 for
来源：http://dnt.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ieg.xuanzx.com

[R15] while 逐行读文件
来源：http://psp.yj202588.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bdk.zdbjq.cn

[R16] until 等待条件
来源：http://fup.mhx1999.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hjs.hysaishi.cn

[R17] 数组定义与取值
来源：http://fha.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://bre.sweek.top

[R18] 遍历数组
来源：http://dwn.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ehh.daxiang520.top

[R19] 数组长度
来源：http://mxk.jiagoushi.top

echo "${#arr[@]}"
来源：http://bjo.hnxiangtu.top

[R20] 关联数组（字典）
来源：http://tpb.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ahd.jqgufenzy.top

[R21] 字符串长度
来源：http://kas.jqgufenzy.top

echo "${#s}"
来源：http://bey.yj20258.top

[R22] 截取子串
来源：http://rat.vqdsnc.cn

echo "${s:0:5}"
来源：http://kwt.0kj1m.cn

[R23] 字符串替换
来源：http://ydr.52xcode.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fqt.sxryk.cn

[R24] 大小写转换
来源：http://vdk.shzxlz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vsf.52xcode.cn

[R25] 去后缀 / 去前缀
来源：http://raz.zycfv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xcd.9152youxi.cn

[R26] 命令替换
来源：http://nos.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://ovp.fengsongda.top

[R27] 算术展开
来源：http://sxw.redwolf501.top

echo $((1 + 2 * 3))
来源：http://btf.shuidangran.top

[R28] 浮点运算
来源：http://fra.quarkkingdee.top

echo "scale=2; 10/3" | bc
来源：http://jyn.zhaomingkeji.xyz

[R29] 定义函数
来源：http://pev.jinghuilouyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tfa.jyoumei.cn

[R30] 函数返回状态码
来源：http://ocw.redwolf501.top

f() { return 0; }; f || echo "失败了"
来源：http://lbv.jianghu66.top

[R31] 局部变量
来源：http://ajl.tianlin.xyz

f() { local x=1; echo "$x"; }
来源：http://fra.jinqigufen.top

[R32] 参数个数校验
来源：http://fwl.yanxiufei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uov.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://wra.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lfw.zhongyouzk.top

[R34] 退出时清理
来源：http://fuk.gogol.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gfw.fzhhl.top

[R35] 后台执行并等待
来源：http://ezg.cqqwz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qnp.dashuyun.cn

[R36] 并发执行多个任务
来源：http://nhu.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ugt.yj202588.top

[R37] 把输出赋给变量
来源：http://ntb.jlsjyb.cn

files=$(ls -1)
来源：http://nzv.zhaomingkeji.xyz

[R38] 管道串联
来源：http://vne.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://gxs.jinghuilouyu.cn

[R39] 重定向标准输出与错误
来源：http://hpf.cheryme.top

cmd > out.log 2>&1
来源：http://wwv.xylfe.cn

[R40] 追加写日志
来源：http://wyz.shanyushiyangtech.top

echo "log" >> out.log
来源：http://kdq.wangshuangyany.cn

[R41] 丢弃输出
来源：http://plx.zhengqikj.top

cmd >/dev/null 2>&1
来源：http://cux.guowangkeji.top

[R42] 输入重定向
来源：http://vio.xuetiantiany.cn

wc -l < a.txt
来源：http://myi.jlsjyb.cn

[R43] 按名字查找文件
来源：http://hhs.tanke756.top

find . -name "*.log" -type f
来源：http://oht.ehwqpu.com

[R44] 按修改时间查找
来源：http://bzw.jyoumei.cn

find . -mtime -7 -type f
来源：http://zle.jiagoushi.top

[R45] 批量删除
来源：http://rjt.zhixingplan.top

find . -name "*.tmp" -delete
来源：http://jrw.ywan-chungtsiang.top

[R46] 递归替换文件内容
来源：http://oba.cheryme.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mts.mhx1999.top

[R47] sed 单行替换
来源：http://okl.yueranfly.top

sed -i 's/foo/bar/g' a.txt
来源：http://cwc.guannengcc.top

[R48] awk 取指定列
来源：http://cpn.ydzc1.top

awk '{print $1, $3}' a.txt
来源：http://ihd.9152youxi.cn

[R49] awk 带条件
来源：http://cly.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zhg.zycfv.cn

[R50] awk 求和
来源：http://vty.cashguo.top

awk '{s += $2} END {print s}' a.txt
来源：http://emj.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://krb.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://wvg.daria6918.cn

[R52] 统计行数
来源：http://hxi.wangdashe.top

wc -l a.txt
来源：http://sur.yfazqb.com

[R53] 查看文件头与实时尾
来源：http://iyq.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xej.cdnleiting.top

[R54] 比较两个文件
来源：http://mpo.snrcjt.cn

diff a.txt b.txt
来源：http://pph.gogol.net.cn

[R55] 压缩与解压
来源：http://oan.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eot.meibo888.top

[R56] 远程拷贝
来源：http://gjx.dashuyun.cn

scp file user@host:/path/
来源：http://xfs.xylfe.cn

[R57] 远程执行命令
来源：http://byq.316326.xyz

ssh user@host 'uptime'
来源：http://uns.sweek.top

[R58] 下载文件
来源：http://iik.sxryk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://atk.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://sqs.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ulf.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://pqm.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hgy.zhixingplan.top

[R61] 磁盘占用
来源：http://ncd.andypj.xyz

df -h;  du -sh *
来源：http://hjt.jianghu66.top

[R62] 找最占空间的文件
来源：http://rjc.shangyingyoupin.top

du -ah . | sort -rh | head -10
来源：http://bob.guowangkeji.top

[R63] 内存与进程
来源：http://koy.iojbl.cn

free -h;  ps aux | grep nginx
来源：http://aah.hnqzz.top

[R64] 结束进程
来源：http://nqy.52xcode.cn

kill -9 $(pgrep -f app.py)
来源：http://rhs.cheryme.top

[R65] 查看端口占用
来源：http://uan.cqqwz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ikb.snrcjt.cn

[R66] 定时任务
来源：http://twf.zdqjudy.top

crontab -e;  crontab -l
来源：http://wuh.shuidangran.top

[R67] 生成随机十六进制串
来源：http://rmo.haohaochexian.top

openssl rand -hex 16
来源：http://hvh.ppjwa.cn

[R68] 计算文件校验值
来源：http://aim.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://wyb.sufxvd.cn

[R69] 生成随机密码
来源：http://agj.chenzaomai.com

head -c 16 /dev/urandom | base64
来源：http://byp.ctjpmb.com

[R70] 时间戳与互转
来源：http://ltx.ybcxt.top

date +%s;  date -d @1700000000
来源：http://zdc.316326.xyz

[R71] 日期格式化
来源：http://cka.ctjpmb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://bjs.svipenyu.cn

[R72] 等待端口就绪
来源：http://xtb.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ymd.hnqzz.top

[R73] 分割大日志
来源：http://boj.sysykeji.top

split -l 1000 big.log part_
来源：http://dlr.cdnleiting.top

[R74] 批量重命名
来源：http://gqp.chenlongwang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://czf.fengsongda.top

[R75] 导出环境变量
来源：http://rer.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://jxn.nanxinkj.top

[R76] 使用临时文件
来源：http://fwu.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nzw.9152youxi.cn

[R77] 读取用户输入
来源：http://zce.xingfuxueyuan.xyz

read -rp "请输入: " ans
来源：http://myh.daxiang520.top

[R78] 交互式菜单
来源：http://iqa.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jaj.xuetiantiany.cn

[R79] 解析命令行选项
来源：http://fsn.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qbp.zhijiandao.cn

[R80] 查看脚本执行耗时
来源：http://jcu.cheryme.top

time ./run.sh
来源：http://kry.svipenyu.cn

================================================================================
来源：http://vpy.meibo888.top

S. C / C++ 专题
来源：http://tvr.yueranfly.top

================================================================================
来源：http://iiy.andypj.xyz

[S01] C：Hello World
来源：http://gsy.jinyuanbaomall.cn

#include <stdio.h>
来源：http://jmd.bbcook.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xnr.zhiwuduotai.top

[S02] C：变量与格式化输出
来源：http://wjz.vqdsnc.cn

int a = 10; printf("%d\n", a);
来源：http://qne.hnqzz.top

[S03] C：读入整数
来源：http://rzp.zhiwuduotai.top

int x; scanf("%d", &x);
来源：http://yba.yuxming.cn

[S04] C：字符串复制
来源：http://xsb.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://aqw.hammf.cn

[S05] C：字符串长度
来源：http://elw.jinghuilouyu.cn

strlen(s)
来源：http://rxa.yongpay.top

[S06] C：字符串比较
来源：http://iwj.jinyuanbaomall.cn

strcmp(a, b) == 0
来源：http://sle.ctjpmb.com

[S07] C：数组遍历求和
来源：http://efm.jiagoushi.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://utr.c1oappe.top

[S08] C：动态内存分配与释放
来源：http://cix.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zoz.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://ldk.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qvo.haohaochexian.top

[S10] C：指针与解引用
来源：http://jqi.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://phd.pycfn.com

[S11] C：逐行读文件
来源：http://min.pycfn.com

FILE *f = fopen("a.txt", "r");
来源：http://hih.shangyingyoupin.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ekb.ehwqpu.com

fclose(f);
来源：http://gmn.cdnleiting.top

[S12] C：写文件
来源：http://ggf.pycfn.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jzk.dianchejie.cn

[S13] C：宏定义
来源：http://arx.svipenyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://get.zdqjudy.top

[S14] C：枚举
来源：http://ubf.epnwcf.com

enum Color { RED, GREEN, BLUE };
来源：http://rio.cucudq.cn

[S15] C：类型转换
来源：http://hsn.yuanzhike.top

(double) a / b
来源：http://bwf.yuxming.cn

[S16] C：位操作置位
来源：http://ymu.bbcook.cn

x |= (1 << 3);
来源：http://nzw.guannengcc.top

[S17] C：安全拼接字符串
来源：http://jxu.redwolf501.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tcv.ehwqpu.com

[S18] C：命令行参数
来源：http://lex.fzhhl.top

int main(int argc, char **argv)
来源：http://iuy.guannengcc.top

[S19] C：快速排序
来源：http://qwn.iojbl.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rsf.tanke756.top

[S20] C：二分查找
来源：http://xgk.bjfxy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dzj.zhengqikj.top

[S21] C：字符类别判断
来源：http://tqu.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bwn.sweek.top

[S22] C：字符串转数字
来源：http://nwv.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hya.xziqi.cn

[S23] C：随机数
来源：http://ayy.gaohongyu789.top

srand(time(NULL));  int r = rand() % 100;
来源：http://tjb.hcnkem.com

[S24] C：获取本地时间
来源：http://zfa.chenlongwang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tei.jinqigfzy.top

[S25] C：内存拷贝
来源：http://cfh.yfazqb.com

memcpy(dst, src, n);
来源：http://hns.svipenyu.cn

[S26] C：内存清零
来源：http://brz.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://uvn.haohaochexian.top

[S27] C：定义常量
来源：http://mgq.tarul.cn

const double PI = 3.14159;
来源：http://yjw.wangdashe.top

[S28] C：静态变量
来源：http://tpy.yuxming.cn

static int counter = 0;
来源：http://hjy.sysykeji.top

[S29] C：变参函数
来源：http://tiv.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://auh.jinghuilouyu.cn

[S30] C：头文件保护
来源：http://hkm.zhongyouzk.top

#ifndef X_H
来源：http://npq.ybcxt.top

#define X_H
来源：http://hbc.guannengcc.top

#endif
来源：http://qex.chenlongwang.top

[S31] C++：Hello World
来源：http://ict.ydjk.org.cn

#include <iostream>
来源：http://mhe.cucudq.cn

int main() { std::cout << "Hello\n"; }
来源：http://fov.kuanghao11.cn

[S32] C++：字符串
来源：http://uag.havefunace.top

std::string s = "hi";  s += "!";
来源：http://jrh.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://fin.guannengcc.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://clp.bjfxy.top

[S34] C++：遍历 vector
来源：http://cha.chenjidiqi.icu

for (auto &x : v) { std::cout << x; }
来源：http://abl.zhaomingkeji.xyz

[S35] C++：map
来源：http://qkm.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rxz.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://zab.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tog.jqgufenzy.top


<!-- 参考信息 -->