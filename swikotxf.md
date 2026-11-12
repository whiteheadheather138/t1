代发 wailian999

SHOW INDEX FROM users;
来源：http://jid.shuidangran.top

[Q73] 查看表状态
来源：http://xfx.jinqigfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://hto.shanyushiyangkeji.top

[Q74] 强制使用索引
来源：http://nwk.tarul.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tmy.c1oappe.top

[Q75] 日期格式化
来源：http://eni.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qok.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pnr.xingfuxueyuan.xyz

[Q76] 按天统计
来源：http://foa.jlsjyb.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zfe.hammf.cn

[Q77] 时间加减
来源：http://jsy.andypj.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mnz.c1oappe.top

[Q78] 当前时间
来源：http://egw.vqdsnc.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://waa.yj20258888.top

[Q79] 字符串拼接
来源：http://dcf.cdnleiting.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mmp.ydzc1.top

[Q80] 字符串截取
来源：http://uvx.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bre.sufxvd.cn

[Q81] 字符串替换
来源：http://ntk.hfpthk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://amp.zdbjq.cn

[Q82] 字符长度与字节长度
来源：http://zvc.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ejz.shuidangran.top

[Q83] 大小写转换
来源：http://vkn.chenjidiqi.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cmi.shangyingyoupin.top

[Q84] 去除首尾空格
来源：http://zdg.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://fsa.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://gzt.tianlin.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tyn.shanyushiyangtech.top

[Q86] 读取 JSON 字段
来源：http://bhs.0kj1m.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ukz.bbcook.cn

[Q87] JSON 字段做条件
来源：http://vtb.jinqigfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qsk.sweek.top

[Q88] 行转列（条件聚合）
来源：http://fnk.iojbl.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ugn.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nsk.pycfn.com

[Q89] 判断表是否存在
来源：http://vfu.chenlongwang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tcm.meibo888.top

[Q90] 生成序号列
来源：http://nvl.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mzg.hfpthk.cn

================================================================================
来源：http://ues.jinyuanbaomall.cn

R. Bash 专题
来源：http://ylz.jqgufenzy.top

================================================================================
来源：http://fsq.yanxiufei.cn

[R01] shebang 与严格模式
来源：http://qph.cashguo.top

#!/usr/bin/env bash
来源：http://cxk.xuanzx.com

set -euo pipefail
来源：http://nsq.aibaodan.cn

[R02] 变量赋值与使用
来源：http://fby.haohaochexian.top

name="Tom"; echo "$name"
来源：http://uha.kuanghao11.cn

[R03] 只读变量
来源：http://gvv.shzxlz.cn

readonly PI=3.14
来源：http://nit.hywenlv.cn

[R04] 位置参数
来源：http://nkj.epnwcf.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gel.jyoumei.cn

[R05] 参数默认值
来源：http://fse.bjfxy.top

name="${1:-default}"
来源：http://dwt.redwolf501.top

[R06] 判断命令是否存在
来源：http://tyi.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ida.yuxming.cn

[R07] if 判断文件
来源：http://uwx.yvedp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sor.yonumen.top

[R08] 数值比较
来源：http://esg.hammf.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://chz.hnxiangtu.top

[R09] 字符串比较
来源：http://amq.fktsv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hce.ivvv.top

[R10] 正则匹配
来源：http://gmi.sufxvd.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pzd.jlsjyb.cn

[R11] case 多分支
来源：http://qwa.aibaodan.cn

case "$1" in
来源：http://tzj.zhoulong.xyz

start) echo "启动" ;;
来源：http://ibc.zycfv.cn

stop)  echo "停止" ;;
来源：http://nso.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://qku.ppjwa.cn

esac
来源：http://meh.meibo888.top

[R12] for 遍历文件
来源：http://qqg.jqgfzy.top

for f in *.txt; do echo "$f"; done
来源：http://gwg.bbcook.cn

[R13] for 计数循环
来源：http://ipa.yongpay.top

for i in {1..10}; do echo "$i"; done
来源：http://iqh.0kj1m.cn

[R14] C 风格 for
来源：http://aam.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yoh.daxiang520.top

[R15] while 逐行读文件
来源：http://rzp.9152youxi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fwe.bjfxy.top

[R16] until 等待条件
来源：http://vis.sweek.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wdc.jinqigfzy.top

[R17] 数组定义与取值
来源：http://umo.daxiang520.top

arr=(a b c); echo "${arr[0]}"
来源：http://mlw.yj20258888.top

[R18] 遍历数组
来源：http://ord.zhengqikj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kid.ctjpmb.com

[R19] 数组长度
来源：http://lfg.jqgfzy.top

echo "${#arr[@]}"
来源：http://cca.bjfxy.top

[R20] 关联数组（字典）
来源：http://jxe.xinyue.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jcy.9152youxi.cn

[R21] 字符串长度
来源：http://duv.nanxuanxn.top

echo "${#s}"
来源：http://pfw.fehbvm.com

[R22] 截取子串
来源：http://jvk.chenzaomai.com

echo "${s:0:5}"
来源：http://qba.quarkkingdee.top

[R23] 字符串替换
来源：http://bjw.nwbrower.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vyz.zycfv.cn

[R24] 大小写转换
来源：http://dom.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://ptq.yfazqb.com

[R25] 去后缀 / 去前缀
来源：http://lbu.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jza.316326.xyz

[R26] 命令替换
来源：http://zfm.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://aea.andypj.xyz

[R27] 算术展开
来源：http://enb.fehbvm.com

echo $((1 + 2 * 3))
来源：http://rkq.yvedp.cn

[R28] 浮点运算
来源：http://fkb.xinyue.icu

echo "scale=2; 10/3" | bc
来源：http://jne.jqgufenzy.top

[R29] 定义函数
来源：http://oit.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wet.gogol.net.cn

[R30] 函数返回状态码
来源：http://ygw.zhaomingkeji.xyz

f() { return 0; }; f || echo "失败了"
来源：http://txb.haohaochexian.top

[R31] 局部变量
来源：http://teq.chenlongwang.top

f() { local x=1; echo "$x"; }
来源：http://wkl.redwolf501.top

[R32] 参数个数校验
来源：http://nli.jinghuilouyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://drb.hcnkem.com

[R33] 捕获错误并提示行号
来源：http://ctq.guowangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://grq.jiagoushi.top

[R34] 退出时清理
来源：http://lqv.0kj1m.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kml.pycfn.com

[R35] 后台执行并等待
来源：http://kmk.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hmq.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://ukg.yj202588.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://abs.ehwqpu.com

[R37] 把输出赋给变量
来源：http://gak.yvedp.cn

files=$(ls -1)
来源：http://wgj.mhx1999.top

[R38] 管道串联
来源：http://ohe.ywan-chungtsiang.top

cat a.txt | grep -i error | wc -l
来源：http://uhe.yvedp.cn

[R39] 重定向标准输出与错误
来源：http://nhf.shuidangran.top

cmd > out.log 2>&1
来源：http://woz.epnwcf.com

[R40] 追加写日志
来源：http://cjy.tanke756.top

echo "log" >> out.log
来源：http://ugr.zhengqikj.top

[R41] 丢弃输出
来源：http://pfj.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://oyy.0kj1m.cn

[R42] 输入重定向
来源：http://lhw.gogol.net.cn

wc -l < a.txt
来源：http://jsw.xuetiantiany.cn

[R43] 按名字查找文件
来源：http://tvg.fanxiaobao.xyz

find . -name "*.log" -type f
来源：http://ill.gotoacloud.top

[R44] 按修改时间查找
来源：http://vwb.vqdsnc.cn

find . -mtime -7 -type f
来源：http://gec.fengsongda.top

[R45] 批量删除
来源：http://thv.birdmap.top

find . -name "*.tmp" -delete
来源：http://vgc.hnxiangtu.top

[R46] 递归替换文件内容
来源：http://bgo.jyoumei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://khh.zhengqikj.top

[R47] sed 单行替换
来源：http://jld.haohaochexian.top

sed -i 's/foo/bar/g' a.txt
来源：http://mcn.yj20258.top

[R48] awk 取指定列
来源：http://uxe.gogol.net.cn

awk '{print $1, $3}' a.txt
来源：http://fnk.hcnkem.com

[R49] awk 带条件
来源：http://zdq.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mgx.hysaishi.cn

[R50] awk 求和
来源：http://uou.jinghuilouyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bpz.yangfankeji.com

[R51] 排序去重取前几
来源：http://kxx.fehbvm.com

sort a.txt | uniq -c | sort -rn | head
来源：http://yjy.vehdjk.com

[R52] 统计行数
来源：http://mvl.chenzaomai.com

wc -l a.txt
来源：http://his.bjfxy.top

[R53] 查看文件头与实时尾
来源：http://kyo.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://san.fehbvm.com

[R54] 比较两个文件
来源：http://qae.cheryme.top

diff a.txt b.txt
来源：http://ydz.ctjpmb.com

[R55] 压缩与解压
来源：http://iey.dianchejie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ynp.shanyushiyangtech.top

[R56] 远程拷贝
来源：http://xyj.tarul.cn

scp file user@host:/path/
来源：http://ljo.ydjk.org.cn

[R57] 远程执行命令
来源：http://mep.mhx1999.top

ssh user@host 'uptime'
来源：http://otk.pycfn.com

[R58] 下载文件
来源：http://dox.zdqjudy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vnk.9152youxi.cn

[R59] 发 POST JSON
来源：http://zvd.jiagoushi.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bpz.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://ecb.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pld.hywenlv.cn

[R61] 磁盘占用
来源：http://gqt.snrcjt.cn

df -h;  du -sh *
来源：http://xzd.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://bkw.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://apc.chenzaomai.com

[R63] 内存与进程
来源：http://ycm.aibaodan.cn

free -h;  ps aux | grep nginx
来源：http://wuz.gogol.net.cn

[R64] 结束进程
来源：http://ecs.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://mdr.c1oappe.top

[R65] 查看端口占用
来源：http://zrg.yangfankeji.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hxj.yonumen.top

[R66] 定时任务
来源：http://ptw.pycfn.com

crontab -e;  crontab -l
来源：http://ies.sysykeji.top

[R67] 生成随机十六进制串
来源：http://tyi.jinghuilouyu.cn

openssl rand -hex 16
来源：http://mdh.aibaodan.cn

[R68] 计算文件校验值
来源：http://jbt.tanke756.top

sha256sum a.txt;  md5sum a.txt
来源：http://eff.quarkkingdee.top

[R69] 生成随机密码
来源：http://qhv.shanyushiyangtech.top

head -c 16 /dev/urandom | base64
来源：http://eim.yj202588.top

[R70] 时间戳与互转
来源：http://hez.shzxlz.cn

date +%s;  date -d @1700000000
来源：http://pqo.ctjpmb.com

[R71] 日期格式化
来源：http://flh.zycfv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hro.ybcxt.top

[R72] 等待端口就绪
来源：http://yfd.guowangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://clu.ctjpmb.com

[R73] 分割大日志
来源：http://ilq.ybcxt.top

split -l 1000 big.log part_
来源：http://tyl.pengpengdd.cyou

[R74] 批量重命名
来源：http://xnm.tarul.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yal.jlsjyb.cn

[R75] 导出环境变量
来源：http://edu.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://iqj.xuetiantiany.cn

[R76] 使用临时文件
来源：http://ciu.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fei.sweek.top

[R77] 读取用户输入
来源：http://tft.shanyushiyangtech.top

read -rp "请输入: " ans
来源：http://whx.guowangkeji.top

[R78] 交互式菜单
来源：http://anh.yfazqb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://rcm.jyoumei.cn

[R79] 解析命令行选项
来源：http://pdf.fzhhl.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cuy.epnwcf.com

[R80] 查看脚本执行耗时
来源：http://bym.ywan-chungtsiang.top

time ./run.sh
来源：http://dtj.hfpthk.cn

================================================================================
来源：http://qbw.xylfe.cn

S. C / C++ 专题
来源：http://ogd.redwolf501.top

================================================================================
来源：http://pxf.aizwys.cn

[S01] C：Hello World
来源：http://rwx.vehdjk.com

#include <stdio.h>
来源：http://msj.chenzaomai.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://xkt.pycfn.com

[S02] C：变量与格式化输出
来源：http://srx.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://iqv.jinghuilouyu.cn

[S03] C：读入整数
来源：http://smq.yvedp.cn

int x; scanf("%d", &x);
来源：http://xcg.sysykeji.top

[S04] C：字符串复制
来源：http://jgd.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://rnt.xylfe.cn

[S05] C：字符串长度
来源：http://fjy.haohaochexian.top

strlen(s)
来源：http://jol.bbcook.cn

[S06] C：字符串比较
来源：http://fkd.316326.xyz

strcmp(a, b) == 0
来源：http://vag.yvedp.cn

[S07] C：数组遍历求和
来源：http://udy.jqgufenzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ndy.jlsjyb.cn

[S08] C：动态内存分配与释放
来源：http://hhf.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wgs.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://gvc.zhixingplan.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pxp.tian-w.cn

[S10] C：指针与解引用
来源：http://fii.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://bpl.bbcook.cn

[S11] C：逐行读文件
来源：http://krl.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://vof.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nxm.yangfankeji.com

fclose(f);
来源：http://nkb.shangyingyoupin.top

[S12] C：写文件
来源：http://ewg.xziqi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ufd.tanke756.top

[S13] C：宏定义
来源：http://lam.chenlongwang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dsm.hysaishi.cn

[S14] C：枚举
来源：http://mbr.sxryk.cn

enum Color { RED, GREEN, BLUE };
来源：http://udr.tianlin.xyz

[S15] C：类型转换
来源：http://wbe.vqdsnc.cn

(double) a / b
来源：http://bgq.tianlin.xyz

[S16] C：位操作置位
来源：http://pjb.xylfe.cn

x |= (1 << 3);
来源：http://ete.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://wfr.ybcxt.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dgq.tanke756.top

[S18] C：命令行参数
来源：http://kxk.shangyingyoupin.top

int main(int argc, char **argv)
来源：http://mlo.ehwqpu.com

[S19] C：快速排序
来源：http://bnc.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://qtt.hysaishi.cn

[S20] C：二分查找
来源：http://lyx.birdmap.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jje.nanxuanxn.top

[S21] C：字符类别判断
来源：http://lyx.cdnleiting.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lwe.aibaodan.cn

[S22] C：字符串转数字
来源：http://cpw.zycfv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yfy.feifeiyinyue.top

[S23] C：随机数
来源：http://vyp.smart0.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://fgf.shzxlz.cn

[S24] C：获取本地时间
来源：http://yjq.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xmn.zdbjq.cn

[S25] C：内存拷贝
来源：http://qwh.dashuyun.cn

memcpy(dst, src, n);
来源：http://lgz.yueranfly.top

[S26] C：内存清零
来源：http://cch.andypj.xyz

memset(a, 0, sizeof a);
来源：http://fmw.redwolf501.top

[S27] C：定义常量
来源：http://pbm.zhengqikj.top

const double PI = 3.14159;
来源：http://djj.daria6918.cn

[S28] C：静态变量
来源：http://kpm.nanxuanxn.top

static int counter = 0;
来源：http://oyi.svipenyu.cn

[S29] C：变参函数
来源：http://knd.9152youxi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mpl.iojbl.cn

[S30] C：头文件保护
来源：http://tpe.c1oappe.top

#ifndef X_H
来源：http://znk.hongshengwenyu.top

#define X_H
来源：http://bbu.zhoulong.xyz

#endif
来源：http://crt.hesvh.cn

[S31] C++：Hello World
来源：http://jqx.zhongyouzk.top

#include <iostream>
来源：http://fuh.tarul.cn

int main() { std::cout << "Hello\n"; }
来源：http://jsd.redwolf501.top

[S32] C++：字符串
来源：http://vqm.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://suf.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://stz.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://upu.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://otl.guowangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://ksh.tanke756.top

[S35] C++：map
来源：http://let.smart0.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bux.jinqigufen.top

[S36] C++：unordered_map
来源：http://tlm.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jde.dashuyun.cn

[S37] C++：set
来源：http://ggu.pengpengdd.cyou

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jbw.ivvv.top

[S38] C++：排序
来源：http://kkn.shanyushiyangkeji.top

std::sort(v.begin(), v.end());
来源：http://qzm.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://ljn.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://onv.ydjk.org.cn

[S40] C++：查找元素
来源：http://cwi.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pnr.cucudq.cn

[S41] C++：类与构造函数
来源：http://jxx.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://klf.jinqigfzy.top

[S42] C++：继承与虚函数
来源：http://cay.yuanzhike.top

class B : public Base { public: void f() override {} };
来源：http://ddi.ydjk.org.cn


<!-- 参考信息 -->