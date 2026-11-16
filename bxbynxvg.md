代发 wailian999

SHOW INDEX FROM users;
来源：http://bug.tarul.cn

[Q73] 查看表状态
来源：http://qnc.ydjk.org.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wzz.haohaochexian.top

[Q74] 强制使用索引
来源：http://dza.xylfe.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zmz.gzhubu.top

[Q75] 日期格式化
来源：http://gsf.vqdsnc.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zvj.xuetiantiany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ojd.yj20258888.top

[Q76] 按天统计
来源：http://iqb.cucudq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zil.zdbjq.cn

[Q77] 时间加减
来源：http://fqn.jqgufenzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pid.pycfn.com

[Q78] 当前时间
来源：http://fmt.c1oappe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://odr.shanyushiyangtech.top

[Q79] 字符串拼接
来源：http://wyz.fktsv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://smp.jinyuanbaomall.cn

[Q80] 字符串截取
来源：http://vah.ivvv.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gmu.andypj.xyz

[Q81] 字符串替换
来源：http://nxr.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vik.feifeiyinyue.top

[Q82] 字符长度与字节长度
来源：http://bcn.chenjidiqi.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bjl.jyoumei.cn

[Q83] 大小写转换
来源：http://bfd.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qdg.vehdjk.com

[Q84] 去除首尾空格
来源：http://wks.haohaochexian.top

SELECT TRIM(name) FROM users;
来源：http://bem.yongpay.top

[Q85] 数值取整
来源：http://bki.gotoacloud.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xkx.birdmap.top

[Q86] 读取 JSON 字段
来源：http://osm.jinqigufen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aie.zhijiandao.cn

[Q87] JSON 字段做条件
来源：http://zpw.sxryk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xrv.zdqjudy.top

[Q88] 行转列（条件聚合）
来源：http://kaa.ydjk.org.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sfb.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xyc.fanxiaobao.xyz

[Q89] 判断表是否存在
来源：http://ygc.zhoulong.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ocs.cheryme.top

[Q90] 生成序号列
来源：http://uqn.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ucp.snrcjt.cn

================================================================================
来源：http://hlh.vqdsnc.cn

R. Bash 专题
来源：http://vis.316326.xyz

================================================================================
来源：http://jzx.xuetiantiany.cn

[R01] shebang 与严格模式
来源：http://uwd.shangyingyoupin.top

#!/usr/bin/env bash
来源：http://lww.jiagoushi.top

set -euo pipefail
来源：http://smo.pycfn.com

[R02] 变量赋值与使用
来源：http://onf.zhiwuduotai.top

name="Tom"; echo "$name"
来源：http://zkt.cucudq.cn

[R03] 只读变量
来源：http://qjy.tarul.cn

readonly PI=3.14
来源：http://ble.yuanzhike.top

[R04] 位置参数
来源：http://xvx.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vqk.nwbrower.top

[R05] 参数默认值
来源：http://zwk.smart0.xyz

name="${1:-default}"
来源：http://azx.pycfn.com

[R06] 判断命令是否存在
来源：http://pup.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ibq.haohaochexian.top

[R07] if 判断文件
来源：http://kud.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dxe.vehdjk.com

[R08] 数值比较
来源：http://ltq.ybcxt.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tzl.hammf.cn

[R09] 字符串比较
来源：http://zvu.yfazqb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dzq.yangfankeji.com

[R10] 正则匹配
来源：http://rce.andypj.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yvh.ywan-chungtsiang.top

[R11] case 多分支
来源：http://yoe.yvedp.cn

case "$1" in
来源：http://bzg.yuanzhike.top

start) echo "启动" ;;
来源：http://fob.shuidangran.top

stop)  echo "停止" ;;
来源：http://aax.hywenlv.cn

*)     echo "未知命令" ;;
来源：http://vli.zdqjudy.top

esac
来源：http://pko.cheryme.top

[R12] for 遍历文件
来源：http://uxn.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://sty.shangyingyoupin.top

[R13] for 计数循环
来源：http://ucl.jqgfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://jox.ctjpmb.com

[R14] C 风格 for
来源：http://xot.hnqzz.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bkr.ybcxt.top

[R15] while 逐行读文件
来源：http://kij.jinyuanbaomall.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://slg.ehwqpu.com

[R16] until 等待条件
来源：http://jmq.shanyushiyangtech.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://awd.chenzaomai.com

[R17] 数组定义与取值
来源：http://ahq.fzhhl.top

arr=(a b c); echo "${arr[0]}"
来源：http://dnb.redwolf501.top

[R18] 遍历数组
来源：http://gro.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qox.chenzaomai.com

[R19] 数组长度
来源：http://pkn.cheryme.top

echo "${#arr[@]}"
来源：http://ryv.fzhhl.top

[R20] 关联数组（字典）
来源：http://qdh.jinyuanbaomall.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lnt.yvedp.cn

[R21] 字符串长度
来源：http://mmd.kuanghao11.cn

echo "${#s}"
来源：http://gxa.yuanzhike.top

[R22] 截取子串
来源：http://wir.hnxiangtu.top

echo "${s:0:5}"
来源：http://ulm.hongshengwenyu.top

[R23] 字符串替换
来源：http://omb.gzhubu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dtl.wangshuangyany.cn

[R24] 大小写转换
来源：http://htb.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://nal.smart0.xyz

[R25] 去后缀 / 去前缀
来源：http://bgq.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fji.jinyuanbaomall.cn

[R26] 命令替换
来源：http://kwx.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://ooc.52xcode.cn

[R27] 算术展开
来源：http://rrn.cashguo.top

echo $((1 + 2 * 3))
来源：http://lbw.guowangkeji.top

[R28] 浮点运算
来源：http://hdk.jianghu66.top

echo "scale=2; 10/3" | bc
来源：http://syj.jyoumei.cn

[R29] 定义函数
来源：http://csy.zycfv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rde.jinqigfzy.top

[R30] 函数返回状态码
来源：http://pim.cdnleiting.top

f() { return 0; }; f || echo "失败了"
来源：http://xwc.wangshuangyany.cn

[R31] 局部变量
来源：http://kjf.9152youxi.cn

f() { local x=1; echo "$x"; }
来源：http://jjl.havefunace.top

[R32] 参数个数校验
来源：http://qul.shanyushiyangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://viw.dashuyun.cn

[R33] 捕获错误并提示行号
来源：http://rli.sysykeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mwa.yuxming.cn

[R34] 退出时清理
来源：http://bed.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://gze.tarul.cn

[R35] 后台执行并等待
来源：http://emz.jinyuanbaomall.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gcb.316326.xyz

[R36] 并发执行多个任务
来源：http://opa.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ici.fanxiaobao.xyz

[R37] 把输出赋给变量
来源：http://piz.hnxiangtu.top

files=$(ls -1)
来源：http://tbm.xuanzx.com

[R38] 管道串联
来源：http://lze.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://zrm.daria6918.cn

[R39] 重定向标准输出与错误
来源：http://jqm.feifeiyinyue.top

cmd > out.log 2>&1
来源：http://nbc.hcnkem.com

[R40] 追加写日志
来源：http://bkt.hammf.cn

echo "log" >> out.log
来源：http://aqn.hongshengwenyu.top

[R41] 丢弃输出
来源：http://zms.yuanzhike.top

cmd >/dev/null 2>&1
来源：http://rtv.jqgufenzy.top

[R42] 输入重定向
来源：http://rbl.bbcook.cn

wc -l < a.txt
来源：http://zat.hfpthk.cn

[R43] 按名字查找文件
来源：http://iqb.zhiwuduotai.top

find . -name "*.log" -type f
来源：http://fjs.meibo888.top

[R44] 按修改时间查找
来源：http://gly.yonumen.top

find . -mtime -7 -type f
来源：http://uih.feifeiyinyue.top

[R45] 批量删除
来源：http://sxj.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://eiz.birdmap.top

[R46] 递归替换文件内容
来源：http://tiz.bjfxy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gin.redwolf501.top

[R47] sed 单行替换
来源：http://hze.fehbvm.com

sed -i 's/foo/bar/g' a.txt
来源：http://urh.zhoulong.xyz

[R48] awk 取指定列
来源：http://wum.zhongyouzk.top

awk '{print $1, $3}' a.txt
来源：http://khn.iojbl.cn

[R49] awk 带条件
来源：http://mjz.ydjk.org.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vtp.tanke756.top

[R50] awk 求和
来源：http://rlu.cucudq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pnv.ppjwa.cn

[R51] 排序去重取前几
来源：http://dlu.jlsjyb.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jid.zdbjq.cn

[R52] 统计行数
来源：http://zaq.jyoumei.cn

wc -l a.txt
来源：http://upu.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://yjl.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fap.xuanzx.com

[R54] 比较两个文件
来源：http://fsl.yfazqb.com

diff a.txt b.txt
来源：http://wog.hysaishi.cn

[R55] 压缩与解压
来源：http://zsq.vqdsnc.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://chz.jinqigfzy.top

[R56] 远程拷贝
来源：http://ncr.jlsjyb.cn

scp file user@host:/path/
来源：http://bpc.gzhubu.top

[R57] 远程执行命令
来源：http://gdb.316326.xyz

ssh user@host 'uptime'
来源：http://qgo.ppjwa.cn

[R58] 下载文件
来源：http://oyv.zhoulong.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kxj.yanxiufei.cn

[R59] 发 POST JSON
来源：http://cmz.jiagoushi.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tup.vqdsnc.cn

[R60] 只看 HTTP 状态码
来源：http://vsh.uphjek.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://amr.hywenlv.cn

[R61] 磁盘占用
来源：http://tdd.sjlbkw.cn

df -h;  du -sh *
来源：http://ltd.guowangkeji.top

[R62] 找最占空间的文件
来源：http://olv.pycfn.com

du -ah . | sort -rh | head -10
来源：http://yfi.zhongyouzk.top

[R63] 内存与进程
来源：http://pru.iojbl.cn

free -h;  ps aux | grep nginx
来源：http://kmn.zhixingplan.top

[R64] 结束进程
来源：http://eec.jinghuilouyu.cn

kill -9 $(pgrep -f app.py)
来源：http://sqv.aibaodan.cn

[R65] 查看端口占用
来源：http://pnt.shuidangran.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ytu.tanke756.top

[R66] 定时任务
来源：http://uwx.ywan-chungtsiang.top

crontab -e;  crontab -l
来源：http://djf.andypj.xyz

[R67] 生成随机十六进制串
来源：http://ydz.xylfe.cn

openssl rand -hex 16
来源：http://oxq.nanxuanxn.top

[R68] 计算文件校验值
来源：http://ayc.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tbn.ehwqpu.com

[R69] 生成随机密码
来源：http://pln.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://eaj.hnxiangtu.top

[R70] 时间戳与互转
来源：http://knp.nwbrower.top

date +%s;  date -d @1700000000
来源：http://eze.chenzaomai.com

[R71] 日期格式化
来源：http://soq.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bsc.cdnleiting.top

[R72] 等待端口就绪
来源：http://lcp.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://rux.52xcode.cn

[R73] 分割大日志
来源：http://upx.andypj.xyz

split -l 1000 big.log part_
来源：http://xax.cucudq.cn

[R74] 批量重命名
来源：http://nzo.tanke756.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ija.ybcxt.top

[R75] 导出环境变量
来源：http://zlt.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://txk.hcnkem.com

[R76] 使用临时文件
来源：http://xmq.sweek.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nka.zhiwuduotai.top

[R77] 读取用户输入
来源：http://vvn.guannengcc.top

read -rp "请输入: " ans
来源：http://gba.cqqwz.cn

[R78] 交互式菜单
来源：http://miy.yvedp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rfc.jianghu66.top

[R79] 解析命令行选项
来源：http://hth.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lcl.gogol.net.cn

[R80] 查看脚本执行耗时
来源：http://wex.ehwqpu.com

time ./run.sh
来源：http://pnt.fktsv.cn

================================================================================
来源：http://jwx.yangfankeji.com

S. C / C++ 专题
来源：http://cva.tarul.cn

================================================================================
来源：http://xpk.cheryme.top

[S01] C：Hello World
来源：http://pym.yueranfly.top

#include <stdio.h>
来源：http://hys.jinqigfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gvy.xinyue.icu

[S02] C：变量与格式化输出
来源：http://gyx.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://cbo.bjfxy.top

[S03] C：读入整数
来源：http://mqs.fzhhl.top

int x; scanf("%d", &x);
来源：http://shi.gotoacloud.top

[S04] C：字符串复制
来源：http://ylk.xingfuxueyuan.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://pbi.havefunace.top

[S05] C：字符串长度
来源：http://dzi.xuetiantiany.cn

strlen(s)
来源：http://hqo.yangfankeji.com

[S06] C：字符串比较
来源：http://jhk.ydjk.org.cn

strcmp(a, b) == 0
来源：http://omo.guowangkeji.top

[S07] C：数组遍历求和
来源：http://uvx.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bam.hfpthk.cn

[S08] C：动态内存分配与释放
来源：http://jig.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fzr.shanyushiyangtech.top

[S09] C：结构体定义与初始化
来源：http://bbe.tanke756.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ebp.jqgfzy.top

[S10] C：指针与解引用
来源：http://jff.ybcxt.top

int *p = &a;  *p = 5;
来源：http://gjx.yfazqb.com

[S11] C：逐行读文件
来源：http://lnt.svipenyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://zhd.bjfxy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://onq.gzhubu.top

fclose(f);
来源：http://wzs.jqgufenzy.top

[S12] C：写文件
来源：http://znx.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zrr.hesvh.cn

[S13] C：宏定义
来源：http://oii.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tjl.yj20258888.top

[S14] C：枚举
来源：http://xht.jlsjyb.cn

enum Color { RED, GREEN, BLUE };
来源：http://fhh.zhongyouzk.top

[S15] C：类型转换
来源：http://edt.chenzaomai.com

(double) a / b
来源：http://vap.redwolf501.top

[S16] C：位操作置位
来源：http://tdl.tianlin.xyz

x |= (1 << 3);
来源：http://cff.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://xoz.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gxp.xylfe.cn

[S18] C：命令行参数
来源：http://pcv.sweek.top

int main(int argc, char **argv)
来源：http://trp.chenjidiqi.icu

[S19] C：快速排序
来源：http://uyw.yangfankeji.com

qsort(a, n, sizeof(int), cmp);
来源：http://rds.yonumen.top

[S20] C：二分查找
来源：http://jkd.nwbrower.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uxb.haohaochexian.top

[S21] C：字符类别判断
来源：http://uqk.epnwcf.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tlt.yueranfly.top

[S22] C：字符串转数字
来源：http://uru.pycfn.com

atoi("42");  strtod("3.14", NULL);
来源：http://cyq.shangyingyoupin.top

[S23] C：随机数
来源：http://oaj.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vse.jlsjyb.cn

[S24] C：获取本地时间
来源：http://wlr.pycfn.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mew.cdnleiting.top

[S25] C：内存拷贝
来源：http://oru.nanxuanxn.top

memcpy(dst, src, n);
来源：http://rho.cqqwz.cn

[S26] C：内存清零
来源：http://eia.shanyushiyangkeji.top

memset(a, 0, sizeof a);
来源：http://cme.hfpthk.cn

[S27] C：定义常量
来源：http://mkq.ppjwa.cn

const double PI = 3.14159;
来源：http://jmp.ydzc1.top

[S28] C：静态变量
来源：http://lwv.vehdjk.com

static int counter = 0;
来源：http://det.gaohongyu789.top

[S29] C：变参函数
来源：http://ehb.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uoh.shzxlz.cn

[S30] C：头文件保护
来源：http://jrq.zhaomingkeji.xyz

#ifndef X_H
来源：http://dls.tanke756.top

#define X_H
来源：http://zmp.redwolf501.top

#endif
来源：http://fpw.bbcook.cn

[S31] C++：Hello World
来源：http://uzh.gogol.net.cn

#include <iostream>
来源：http://lgv.vqdsnc.cn

int main() { std::cout << "Hello\n"; }
来源：http://ghu.yueranfly.top

[S32] C++：字符串
来源：http://ary.xingfuxueyuan.xyz

std::string s = "hi";  s += "!";
来源：http://qyu.jinghuilouyu.cn

[S33] C++：vector 增删
来源：http://uok.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kig.haohaochexian.top

[S34] C++：遍历 vector
来源：http://ruf.yj20258.top

for (auto &x : v) { std::cout << x; }
来源：http://vaq.zhongyouzk.top

[S35] C++：map
来源：http://gse.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dlf.gzhubu.top

[S36] C++：unordered_map
来源：http://pdo.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ymx.bbcook.cn

[S37] C++：set
来源：http://jci.chenzaomai.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wbf.daria6918.cn

[S38] C++：排序
来源：http://agb.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://jbo.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://cgz.birdmap.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xlv.52xcode.cn

[S40] C++：查找元素
来源：http://aop.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lmq.uphjek.com

[S41] C++：类与构造函数
来源：http://qjw.jianghu66.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gvp.hesvh.cn

[S42] C++：继承与虚函数
来源：http://hqn.ywan-chungtsiang.top

class B : public Base { public: void f() override {} };
来源：http://nwq.sufxvd.cn


<!-- 参考信息 -->