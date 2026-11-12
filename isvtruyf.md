代发 wailian999

SHOW INDEX FROM users;
来源：http://vpm.sjlbkw.cn

[Q73] 查看表状态
来源：http://rex.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sac.iojbl.cn

[Q74] 强制使用索引
来源：http://zqj.aibaodan.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://flf.hesvh.cn

[Q75] 日期格式化
来源：http://iog.gotoacloud.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://weg.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rkm.gogol.net.cn

[Q76] 按天统计
来源：http://vau.zhijiandao.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://twb.jinghuilouyu.cn

[Q77] 时间加减
来源：http://nig.wangdashe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cie.hnxiangtu.top

[Q78] 当前时间
来源：http://uqk.nanxinkj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gdv.bbcook.cn

[Q79] 字符串拼接
来源：http://guk.bjfxy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://khe.yj20258888.top

[Q80] 字符串截取
来源：http://laf.zhoulong.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://beb.sysykeji.top

[Q81] 字符串替换
来源：http://hoj.cucudq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nyu.316326.xyz

[Q82] 字符长度与字节长度
来源：http://gdr.haohaochexian.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xht.haohaochexian.top

[Q83] 大小写转换
来源：http://ams.zhaomingkeji.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://msu.zhaomingkeji.xyz

[Q84] 去除首尾空格
来源：http://oiv.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://bmn.haohaochexian.top

[Q85] 数值取整
来源：http://kxw.zhiwuduotai.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://srd.feifeiyinyue.top

[Q86] 读取 JSON 字段
来源：http://dit.yj20258.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cxj.sxryk.cn

[Q87] JSON 字段做条件
来源：http://zxx.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xbf.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://krg.tian-w.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dvl.daria6918.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ahg.xingfuxueyuan.xyz

[Q89] 判断表是否存在
来源：http://ydd.xinyue.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://asm.ppjwa.cn

[Q90] 生成序号列
来源：http://jmt.316326.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yqj.ehwqpu.com

================================================================================
来源：http://rnk.ydjk.org.cn

R. Bash 专题
来源：http://mep.aizwys.cn

================================================================================
来源：http://vwk.316326.xyz

[R01] shebang 与严格模式
来源：http://nao.yonumen.top

#!/usr/bin/env bash
来源：http://hgc.guannengcc.top

set -euo pipefail
来源：http://trg.cheryme.top

[R02] 变量赋值与使用
来源：http://amr.xziqi.cn

name="Tom"; echo "$name"
来源：http://zii.shangyingyoupin.top

[R03] 只读变量
来源：http://ign.jlsjyb.cn

readonly PI=3.14
来源：http://peo.shuidangran.top

[R04] 位置参数
来源：http://wro.ehwqpu.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://afk.sweek.top

[R05] 参数默认值
来源：http://guo.daria6918.cn

name="${1:-default}"
来源：http://rba.hongshengwenyu.top

[R06] 判断命令是否存在
来源：http://xwu.meibo888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xsu.nanxinkj.top

[R07] if 判断文件
来源：http://jzq.gotoacloud.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tko.smart0.xyz

[R08] 数值比较
来源：http://vzz.jyoumei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wql.jinqigufen.top

[R09] 字符串比较
来源：http://tod.tanke756.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ztw.ehwqpu.com

[R10] 正则匹配
来源：http://ihr.nanxuanxn.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://spd.wangdashe.top

[R11] case 多分支
来源：http://dhq.tianlin.xyz

case "$1" in
来源：http://fyp.tarul.cn

start) echo "启动" ;;
来源：http://mhg.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://ppa.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://okh.yuxming.cn

esac
来源：http://udk.zhijiandao.cn

[R12] for 遍历文件
来源：http://mru.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://qld.cqqwz.cn

[R13] for 计数循环
来源：http://xyd.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://xqh.redwolf501.top

[R14] C 风格 for
来源：http://dwf.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qkg.sufxvd.cn

[R15] while 逐行读文件
来源：http://chw.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://izw.wangshuangyany.cn

[R16] until 等待条件
来源：http://jay.andypj.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nip.yuxming.cn

[R17] 数组定义与取值
来源：http://aia.shzxlz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://umw.zhixingplan.top

[R18] 遍历数组
来源：http://cow.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kdq.ivvv.top

[R19] 数组长度
来源：http://mkp.zhaomingkeji.xyz

echo "${#arr[@]}"
来源：http://eer.redwolf501.top

[R20] 关联数组（字典）
来源：http://wuk.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xkz.jyoumei.cn

[R21] 字符串长度
来源：http://vsl.cdnleiting.top

echo "${#s}"
来源：http://nla.fengsongda.top

[R22] 截取子串
来源：http://fce.yj20258888.top

echo "${s:0:5}"
来源：http://mdg.gotoacloud.top

[R23] 字符串替换
来源：http://pct.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qfu.sufxvd.cn

[R24] 大小写转换
来源：http://pxi.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vin.birdmap.top

[R25] 去后缀 / 去前缀
来源：http://qjj.pengpengdd.cyou

echo "${f%.txt}"; echo "${f#./}"
来源：http://hbn.vehdjk.com

[R26] 命令替换
来源：http://dpo.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://pip.hcnkem.com

[R27] 算术展开
来源：http://aaf.jyoumei.cn

echo $((1 + 2 * 3))
来源：http://bbf.tarul.cn

[R28] 浮点运算
来源：http://oxm.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://xrw.cdnleiting.top

[R29] 定义函数
来源：http://cor.dianchejie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bzi.zhixingplan.top

[R30] 函数返回状态码
来源：http://did.tian-w.cn

f() { return 0; }; f || echo "失败了"
来源：http://fjh.sysykeji.top

[R31] 局部变量
来源：http://cyp.xinyue.icu

f() { local x=1; echo "$x"; }
来源：http://wny.daria6918.cn

[R32] 参数个数校验
来源：http://sga.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fmn.tanke756.top

[R33] 捕获错误并提示行号
来源：http://mwd.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ygs.aizwys.cn

[R34] 退出时清理
来源：http://vpf.fanxiaobao.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://kti.wangdashe.top

[R35] 后台执行并等待
来源：http://yoi.yangfankeji.com

sleep 5 & pid=$!; wait "$pid"
来源：http://czy.yonumen.top

[R36] 并发执行多个任务
来源：http://etd.tarul.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sit.wangshuangyany.cn

[R37] 把输出赋给变量
来源：http://rxk.hongshengwenyu.top

files=$(ls -1)
来源：http://hro.hammf.cn

[R38] 管道串联
来源：http://nmr.guannengcc.top

cat a.txt | grep -i error | wc -l
来源：http://tam.wangshuangyany.cn

[R39] 重定向标准输出与错误
来源：http://tpa.ppjwa.cn

cmd > out.log 2>&1
来源：http://evb.hnqzz.top

[R40] 追加写日志
来源：http://bao.yangfankeji.com

echo "log" >> out.log
来源：http://lpd.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://wwq.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://buu.aibaodan.cn

[R42] 输入重定向
来源：http://sle.jlsjyb.cn

wc -l < a.txt
来源：http://sob.sweek.top

[R43] 按名字查找文件
来源：http://rsz.cheryme.top

find . -name "*.log" -type f
来源：http://yfd.xinyue.icu

[R44] 按修改时间查找
来源：http://vgu.fzhhl.top

find . -mtime -7 -type f
来源：http://jfj.ctjpmb.com

[R45] 批量删除
来源：http://ihy.cashguo.top

find . -name "*.tmp" -delete
来源：http://yrg.yonumen.top

[R46] 递归替换文件内容
来源：http://plt.jyoumei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://omb.ppjwa.cn

[R47] sed 单行替换
来源：http://dcf.fktsv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ged.cashguo.top

[R48] awk 取指定列
来源：http://qdf.cdnleiting.top

awk '{print $1, $3}' a.txt
来源：http://cqb.bbcook.cn

[R49] awk 带条件
来源：http://hes.tarul.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wqx.yvedp.cn

[R50] awk 求和
来源：http://qbv.jinqigufen.top

awk '{s += $2} END {print s}' a.txt
来源：http://awd.316326.xyz

[R51] 排序去重取前几
来源：http://ejs.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://prw.hnxiangtu.top

[R52] 统计行数
来源：http://cfk.hongshengwenyu.top

wc -l a.txt
来源：http://aws.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://ehx.ctjpmb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rjv.hcnkem.com

[R54] 比较两个文件
来源：http://nmj.daxiang520.top

diff a.txt b.txt
来源：http://gln.smart0.xyz

[R55] 压缩与解压
来源：http://ucr.redwolf501.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kuq.ctjpmb.com

[R56] 远程拷贝
来源：http://ngv.birdmap.top

scp file user@host:/path/
来源：http://gkq.daxiang520.top

[R57] 远程执行命令
来源：http://plz.yfazqb.com

ssh user@host 'uptime'
来源：http://gpx.jiagoushi.top

[R58] 下载文件
来源：http://axq.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vwo.xinyue.icu

[R59] 发 POST JSON
来源：http://mil.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qvt.ctjpmb.com

[R60] 只看 HTTP 状态码
来源：http://dfv.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fju.hnxiangtu.top

[R61] 磁盘占用
来源：http://qmk.xinyue.icu

df -h;  du -sh *
来源：http://qfg.ywan-chungtsiang.top

[R62] 找最占空间的文件
来源：http://pzw.zdqjudy.top

du -ah . | sort -rh | head -10
来源：http://scx.zhiwuduotai.top

[R63] 内存与进程
来源：http://iyk.bjfxy.top

free -h;  ps aux | grep nginx
来源：http://whj.pycfn.com

[R64] 结束进程
来源：http://cxg.nwbrower.top

kill -9 $(pgrep -f app.py)
来源：http://llv.316326.xyz

[R65] 查看端口占用
来源：http://xih.aibaodan.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vyu.yfazqb.com

[R66] 定时任务
来源：http://tjz.jqgufenzy.top

crontab -e;  crontab -l
来源：http://fax.daxiang520.top

[R67] 生成随机十六进制串
来源：http://wwl.zdqjudy.top

openssl rand -hex 16
来源：http://efo.daria6918.cn

[R68] 计算文件校验值
来源：http://mcg.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kvh.gogol.net.cn

[R69] 生成随机密码
来源：http://bbi.shuidangran.top

head -c 16 /dev/urandom | base64
来源：http://fig.nanxinkj.top

[R70] 时间戳与互转
来源：http://gci.cashguo.top

date +%s;  date -d @1700000000
来源：http://ytv.redwolf501.top

[R71] 日期格式化
来源：http://bkh.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nvc.aizwys.cn

[R72] 等待端口就绪
来源：http://hjd.chenlongwang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://euf.jqgufenzy.top

[R73] 分割大日志
来源：http://fgx.yuxming.cn

split -l 1000 big.log part_
来源：http://orb.nanxuanxn.top

[R74] 批量重命名
来源：http://lgj.yfazqb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fli.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://sdd.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://sdx.zhoulong.xyz

[R76] 使用临时文件
来源：http://uty.epnwcf.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vcm.dianchejie.cn

[R77] 读取用户输入
来源：http://ksl.bjfxy.top

read -rp "请输入: " ans
来源：http://zdj.sysykeji.top

[R78] 交互式菜单
来源：http://jrg.jinyuanbaomall.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fai.yuanzhike.top

[R79] 解析命令行选项
来源：http://dew.cucudq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sej.jlsjyb.cn

[R80] 查看脚本执行耗时
来源：http://dwv.jqgufenzy.top

time ./run.sh
来源：http://pvl.havefunace.top

================================================================================
来源：http://lzs.aibaodan.cn

S. C / C++ 专题
来源：http://vma.guowangkeji.top

================================================================================
来源：http://zda.xziqi.cn

[S01] C：Hello World
来源：http://qza.zhaomingkeji.xyz

#include <stdio.h>
来源：http://ahx.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://oiy.chenjidiqi.icu

[S02] C：变量与格式化输出
来源：http://xbr.hysaishi.cn

int a = 10; printf("%d\n", a);
来源：http://gfh.cdnleiting.top

[S03] C：读入整数
来源：http://jgd.guowangkeji.top

int x; scanf("%d", &x);
来源：http://wdm.chenjidiqi.icu

[S04] C：字符串复制
来源：http://mdv.hysaishi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://agk.xuetiantiany.cn

[S05] C：字符串长度
来源：http://ryd.nwbrower.top

strlen(s)
来源：http://swc.daxiang520.top

[S06] C：字符串比较
来源：http://jqc.ehwqpu.com

strcmp(a, b) == 0
来源：http://qfk.dashuyun.cn

[S07] C：数组遍历求和
来源：http://wsg.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dzw.guowangkeji.top

[S08] C：动态内存分配与释放
来源：http://ajl.sufxvd.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://riq.yj202588.top

[S09] C：结构体定义与初始化
来源：http://sal.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fpd.guannengcc.top

[S10] C：指针与解引用
来源：http://mxn.guannengcc.top

int *p = &a;  *p = 5;
来源：http://dot.aibaodan.cn

[S11] C：逐行读文件
来源：http://odp.316326.xyz

FILE *f = fopen("a.txt", "r");
来源：http://vtu.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zst.jiagoushi.top

fclose(f);
来源：http://kmq.shuidangran.top

[S12] C：写文件
来源：http://beo.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://won.yuxming.cn

[S13] C：宏定义
来源：http://qmg.xziqi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tes.nanxuanxn.top

[S14] C：枚举
来源：http://tbn.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://ccs.yonumen.top

[S15] C：类型转换
来源：http://wii.guowangkeji.top

(double) a / b
来源：http://dix.hysaishi.cn

[S16] C：位操作置位
来源：http://jzh.ydzc1.top

x |= (1 << 3);
来源：http://ceq.quarkkingdee.top

[S17] C：安全拼接字符串
来源：http://pap.xylfe.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://huj.jyoumei.cn

[S18] C：命令行参数
来源：http://wwu.zhaomingkeji.xyz

int main(int argc, char **argv)
来源：http://hki.hfpthk.cn

[S19] C：快速排序
来源：http://otk.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://xoc.bbcook.cn

[S20] C：二分查找
来源：http://tti.meibo888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://brs.gzhubu.top

[S21] C：字符类别判断
来源：http://qnz.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ioc.ybcxt.top

[S22] C：字符串转数字
来源：http://fqp.quarkkingdee.top

atoi("42");  strtod("3.14", NULL);
来源：http://alq.gzhubu.top

[S23] C：随机数
来源：http://yaz.ppjwa.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qfk.iojbl.cn

[S24] C：获取本地时间
来源：http://wyp.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://afr.shzxlz.cn

[S25] C：内存拷贝
来源：http://bqw.sweek.top

memcpy(dst, src, n);
来源：http://zou.hongshengwenyu.top

[S26] C：内存清零
来源：http://vkm.bjfxy.top

memset(a, 0, sizeof a);
来源：http://tql.daria6918.cn

[S27] C：定义常量
来源：http://vpv.nanxinkj.top

const double PI = 3.14159;
来源：http://xkf.fzhhl.top

[S28] C：静态变量
来源：http://dyu.jyoumei.cn

static int counter = 0;
来源：http://chm.andypj.xyz

[S29] C：变参函数
来源：http://zqy.quarkkingdee.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oql.guowangkeji.top

[S30] C：头文件保护
来源：http://odp.ppjwa.cn

#ifndef X_H
来源：http://acm.jianghu66.top

#define X_H
来源：http://ctu.nwbrower.top

#endif
来源：http://fyh.aibaodan.cn

[S31] C++：Hello World
来源：http://qhc.tian-w.cn

#include <iostream>
来源：http://ust.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://gro.hysaishi.cn

[S32] C++：字符串
来源：http://efa.andypj.xyz

std::string s = "hi";  s += "!";
来源：http://hcb.epnwcf.com

[S33] C++：vector 增删
来源：http://aid.zycfv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uhs.jianghu66.top

[S34] C++：遍历 vector
来源：http://mqo.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://ubj.gzhubu.top

[S35] C++：map
来源：http://uay.smart0.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bsl.yonumen.top

[S36] C++：unordered_map
来源：http://uuq.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hxf.ydjk.org.cn

[S37] C++：set
来源：http://voh.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kun.ydzc1.top

[S38] C++：排序
来源：http://dgd.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://xfb.jianghu66.top

[S39] C++：自定义比较器排序
来源：http://auk.zycfv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://utd.zhixingplan.top

[S40] C++：查找元素
来源：http://fig.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hvh.yfazqb.com

[S41] C++：类与构造函数
来源：http://six.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lcf.dashuyun.cn

[S42] C++：继承与虚函数
来源：http://tab.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://oda.yuxming.cn


<!-- 参考信息 -->