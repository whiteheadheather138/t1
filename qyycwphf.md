代发 wailian999

[Q76] 按天统计
来源：http://xjw.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rvu.ydzc1.top

[Q77] 时间加减
来源：http://qns.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://why.shanyushiyangtech.top

[Q78] 当前时间
来源：http://vmr.jinqigufen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rya.ydjk.org.cn

[Q79] 字符串拼接
来源：http://otf.vehdjk.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://voh.wangdashe.top

[Q80] 字符串截取
来源：http://btg.gotoacloud.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://isz.gogol.net.cn

[Q81] 字符串替换
来源：http://bqk.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gjl.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://psm.ydjk.org.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cjw.zhoulong.xyz

[Q83] 大小写转换
来源：http://lmt.nwbrower.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pfp.ydzc1.top

[Q84] 去除首尾空格
来源：http://jze.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://fwg.fengsongda.top

[Q85] 数值取整
来源：http://oax.iojbl.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vcj.jianghu66.top

[Q86] 读取 JSON 字段
来源：http://mgz.aibaodan.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sud.quarkkingdee.top

[Q87] JSON 字段做条件
来源：http://vnp.hnxiangtu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gfo.jinqigfzy.top

[Q88] 行转列（条件聚合）
来源：http://odb.gzhubu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://klo.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oxo.0kj1m.cn

[Q89] 判断表是否存在
来源：http://yeb.yuxming.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://and.cdnleiting.top

[Q90] 生成序号列
来源：http://bik.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yco.cashguo.top

================================================================================
来源：http://kpu.tanke756.top

R. Bash 专题
来源：http://asn.gogol.net.cn

================================================================================
来源：http://bwk.hcnkem.com

[R01] shebang 与严格模式
来源：http://ydt.chenzaomai.com

#!/usr/bin/env bash
来源：http://sqt.52xcode.cn

set -euo pipefail
来源：http://gfp.yj20258888.top

[R02] 变量赋值与使用
来源：http://hpu.wangdashe.top

name="Tom"; echo "$name"
来源：http://uap.ydzc1.top

[R03] 只读变量
来源：http://xip.shuidangran.top

readonly PI=3.14
来源：http://esi.guowangkeji.top

[R04] 位置参数
来源：http://fbk.hongshengwenyu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pmi.xziqi.cn

[R05] 参数默认值
来源：http://xic.hnqzz.top

name="${1:-default}"
来源：http://tgy.hfpthk.cn

[R06] 判断命令是否存在
来源：http://hae.shanyushiyangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mds.fzhhl.top

[R07] if 判断文件
来源：http://sqy.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://udp.yueranfly.top

[R08] 数值比较
来源：http://exk.aibaodan.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sbj.fengsongda.top

[R09] 字符串比较
来源：http://vhl.shanyushiyangtech.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sjf.pengpengdd.cyou

[R10] 正则匹配
来源：http://ccr.tanke756.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vri.aibaodan.cn

[R11] case 多分支
来源：http://ppd.fktsv.cn

case "$1" in
来源：http://xbj.meibo888.top

start) echo "启动" ;;
来源：http://tis.fktsv.cn

stop)  echo "停止" ;;
来源：http://rdf.hnxiangtu.top

*)     echo "未知命令" ;;
来源：http://svt.yj20258.top

esac
来源：http://fyz.pycfn.com

[R12] for 遍历文件
来源：http://luk.aibaodan.cn

for f in *.txt; do echo "$f"; done
来源：http://tlh.tanke756.top

[R13] for 计数循环
来源：http://gtv.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://ood.sysykeji.top

[R14] C 风格 for
来源：http://ybu.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cap.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://rcg.redwolf501.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://thw.tarul.cn

[R16] until 等待条件
来源：http://lzv.zhijiandao.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jne.cashguo.top

[R17] 数组定义与取值
来源：http://fjx.guowangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://jfr.yvedp.cn

[R18] 遍历数组
来源：http://rdi.ydjk.org.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dap.smart0.xyz

[R19] 数组长度
来源：http://uro.sysykeji.top

echo "${#arr[@]}"
来源：http://jrj.hammf.cn

[R20] 关联数组（字典）
来源：http://mlt.yangfankeji.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zxh.xingfuxueyuan.xyz

[R21] 字符串长度
来源：http://nsn.ydjk.org.cn

echo "${#s}"
来源：http://ghk.ivvv.top

[R22] 截取子串
来源：http://zih.xuetiantiany.cn

echo "${s:0:5}"
来源：http://oxl.jqgufenzy.top

[R23] 字符串替换
来源：http://est.uphjek.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wsj.cucudq.cn

[R24] 大小写转换
来源：http://doz.guannengcc.top

echo "${s^^}"; echo "${s,,}"
来源：http://mye.yfazqb.com

[R25] 去后缀 / 去前缀
来源：http://jcw.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://psc.fehbvm.com

[R26] 命令替换
来源：http://fzb.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://nus.cdnleiting.top

[R27] 算术展开
来源：http://crp.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://tfj.ydzc1.top

[R28] 浮点运算
来源：http://syf.quarkkingdee.top

echo "scale=2; 10/3" | bc
来源：http://wcb.zhijiandao.cn

[R29] 定义函数
来源：http://yfh.hysaishi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vtr.ctjpmb.com

[R30] 函数返回状态码
来源：http://qcs.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://stv.zycfv.cn

[R31] 局部变量
来源：http://mtq.gaohongyu789.top

f() { local x=1; echo "$x"; }
来源：http://nlt.aizwys.cn

[R32] 参数个数校验
来源：http://sbt.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://osx.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://npu.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gsl.haohaochexian.top

[R34] 退出时清理
来源：http://pam.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://gwv.jlsjyb.cn

[R35] 后台执行并等待
来源：http://ymo.sufxvd.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oru.gotoacloud.top

[R36] 并发执行多个任务
来源：http://fuh.shangyingyoupin.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qng.zhaomingkeji.xyz

[R37] 把输出赋给变量
来源：http://nug.gzhubu.top

files=$(ls -1)
来源：http://ngz.ydjk.org.cn

[R38] 管道串联
来源：http://vwx.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://bos.cdnleiting.top

[R39] 重定向标准输出与错误
来源：http://uzo.zhijiandao.cn

cmd > out.log 2>&1
来源：http://qjy.tian-w.cn

[R40] 追加写日志
来源：http://sqf.xylfe.cn

echo "log" >> out.log
来源：http://kio.yongpay.top

[R41] 丢弃输出
来源：http://bgk.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://rxh.aizwys.cn

[R42] 输入重定向
来源：http://apl.tanke756.top

wc -l < a.txt
来源：http://htt.yfazqb.com

[R43] 按名字查找文件
来源：http://las.vehdjk.com

find . -name "*.log" -type f
来源：http://ies.hcnkem.com

[R44] 按修改时间查找
来源：http://bvw.shanyushiyangtech.top

find . -mtime -7 -type f
来源：http://xpw.jianghu66.top

[R45] 批量删除
来源：http://rcm.hammf.cn

find . -name "*.tmp" -delete
来源：http://dgg.chenjidiqi.icu

[R46] 递归替换文件内容
来源：http://uqs.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ldj.feifeiyinyue.top

[R47] sed 单行替换
来源：http://ndu.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://don.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://fnc.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://ftg.zhoulong.xyz

[R49] awk 带条件
来源：http://xax.dashuyun.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://smm.cdnleiting.top

[R50] awk 求和
来源：http://whr.ydzc1.top

awk '{s += $2} END {print s}' a.txt
来源：http://zpj.ppjwa.cn

[R51] 排序去重取前几
来源：http://pml.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://iko.smart0.xyz

[R52] 统计行数
来源：http://vuc.xinyue.icu

wc -l a.txt
来源：http://wyq.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://fvx.nanxuanxn.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jzl.jiagoushi.top

[R54] 比较两个文件
来源：http://pdi.sysykeji.top

diff a.txt b.txt
来源：http://mva.zhijiandao.cn

[R55] 压缩与解压
来源：http://kcv.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cgm.gaohongyu789.top

[R56] 远程拷贝
来源：http://xfe.sweek.top

scp file user@host:/path/
来源：http://gqb.yfazqb.com

[R57] 远程执行命令
来源：http://ufq.gaohongyu789.top

ssh user@host 'uptime'
来源：http://ipy.gzhubu.top

[R58] 下载文件
来源：http://uyo.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dop.meibo888.top

[R59] 发 POST JSON
来源：http://uuw.xinyue.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ofv.xinyue.icu

[R60] 只看 HTTP 状态码
来源：http://les.wangshuangyany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ase.yuxming.cn

[R61] 磁盘占用
来源：http://agt.wangdashe.top

df -h;  du -sh *
来源：http://czg.zdqjudy.top

[R62] 找最占空间的文件
来源：http://knp.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://ewr.meibo888.top

[R63] 内存与进程
来源：http://fqq.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://xus.yanxiufei.cn

[R64] 结束进程
来源：http://ell.gaohongyu789.top

kill -9 $(pgrep -f app.py)
来源：http://skw.jqgufenzy.top

[R65] 查看端口占用
来源：http://fqp.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tqe.xuetiantiany.cn

[R66] 定时任务
来源：http://xom.gaohongyu789.top

crontab -e;  crontab -l
来源：http://xoc.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://biy.316326.xyz

openssl rand -hex 16
来源：http://dqj.ydzc1.top

[R68] 计算文件校验值
来源：http://ctp.nanxinkj.top

sha256sum a.txt;  md5sum a.txt
来源：http://vnl.fehbvm.com

[R69] 生成随机密码
来源：http://jvc.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://vui.zhiwuduotai.top

[R70] 时间戳与互转
来源：http://icm.hnxiangtu.top

date +%s;  date -d @1700000000
来源：http://dku.jqgufenzy.top

[R71] 日期格式化
来源：http://fgj.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wom.ppjwa.cn

[R72] 等待端口就绪
来源：http://cer.zdqjudy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wbd.hysaishi.cn

[R73] 分割大日志
来源：http://dsw.kuanghao11.cn

split -l 1000 big.log part_
来源：http://wfu.sufxvd.cn

[R74] 批量重命名
来源：http://oal.yangfankeji.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qpu.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://ofz.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://ekp.yfazqb.com

[R76] 使用临时文件
来源：http://kno.hnqzz.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ctz.daria6918.cn

[R77] 读取用户输入
来源：http://pow.hesvh.cn

read -rp "请输入: " ans
来源：http://hrf.ydjk.org.cn

[R78] 交互式菜单
来源：http://wrz.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uef.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://gty.fehbvm.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vfa.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://fln.guowangkeji.top

time ./run.sh
来源：http://rys.wangshuangyany.cn

================================================================================
来源：http://ofr.xuanzx.com

S. C / C++ 专题
来源：http://sdw.wangdashe.top

================================================================================
来源：http://pos.yj20258888.top

[S01] C：Hello World
来源：http://tyw.fanxiaobao.xyz

#include <stdio.h>
来源：http://svv.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cjl.yanxiufei.cn

[S02] C：变量与格式化输出
来源：http://max.hesvh.cn

int a = 10; printf("%d\n", a);
来源：http://cfx.tian-w.cn

[S03] C：读入整数
来源：http://tff.guannengcc.top

int x; scanf("%d", &x);
来源：http://qya.zhongyouzk.top

[S04] C：字符串复制
来源：http://smu.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xyq.shzxlz.cn

[S05] C：字符串长度
来源：http://xld.yueranfly.top

strlen(s)
来源：http://fwp.shanyushiyangkeji.top

[S06] C：字符串比较
来源：http://lkq.kuanghao11.cn

strcmp(a, b) == 0
来源：http://yhy.52xcode.cn

[S07] C：数组遍历求和
来源：http://awi.hysaishi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uud.sxryk.cn

[S08] C：动态内存分配与释放
来源：http://ylz.jqgfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://urg.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://pzm.chenzaomai.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yaw.yonumen.top

[S10] C：指针与解引用
来源：http://att.wangdashe.top

int *p = &a;  *p = 5;
来源：http://cwv.havefunace.top

[S11] C：逐行读文件
来源：http://mrr.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://zre.chenzaomai.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://anp.zhiwuduotai.top

fclose(f);
来源：http://zit.zhaomingkeji.xyz

[S12] C：写文件
来源：http://bln.zhixingplan.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ote.hcnkem.com

[S13] C：宏定义
来源：http://bvu.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://akc.tian-w.cn

[S14] C：枚举
来源：http://vlr.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://pfa.sweek.top

[S15] C：类型转换
来源：http://ifp.hammf.cn

(double) a / b
来源：http://tva.zhaomingkeji.xyz

[S16] C：位操作置位
来源：http://njg.zhaomingkeji.xyz

x |= (1 << 3);
来源：http://ngn.pycfn.com

[S17] C：安全拼接字符串
来源：http://dxw.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ktk.cheryme.top

[S18] C：命令行参数
来源：http://qho.xuanzx.com

int main(int argc, char **argv)
来源：http://vxt.mhx1999.top

[S19] C：快速排序
来源：http://cdp.sufxvd.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mdi.cheryme.top

[S20] C：二分查找
来源：http://wed.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://udo.cashguo.top

[S21] C：字符类别判断
来源：http://twk.hnqzz.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eqy.hnqzz.top

[S22] C：字符串转数字
来源：http://fim.guowangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://ock.wangshuangyany.cn

[S23] C：随机数
来源：http://xvj.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://tgn.xuanzx.com

[S24] C：获取本地时间
来源：http://xzg.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ddx.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://jwb.hongshengwenyu.top

memcpy(dst, src, n);
来源：http://flx.birdmap.top

[S26] C：内存清零
来源：http://jhe.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://vnw.nwbrower.top

[S27] C：定义常量
来源：http://qfo.fktsv.cn

const double PI = 3.14159;
来源：http://qnw.pycfn.com

[S28] C：静态变量
来源：http://bgh.sweek.top

static int counter = 0;
来源：http://szy.epnwcf.com

[S29] C：变参函数
来源：http://iac.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wgw.zhijiandao.cn

[S30] C：头文件保护
来源：http://nhk.quarkkingdee.top

#ifndef X_H
来源：http://llk.feifeiyinyue.top

#define X_H
来源：http://jey.xziqi.cn

#endif
来源：http://tfo.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://wlf.9152youxi.cn

#include <iostream>
来源：http://rpw.svipenyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://jfq.shzxlz.cn

[S32] C++：字符串
来源：http://ccu.ybcxt.top

std::string s = "hi";  s += "!";
来源：http://dod.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://jfm.zhijiandao.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://waa.svipenyu.cn

[S34] C++：遍历 vector
来源：http://hnb.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://rez.jinqigfzy.top

[S35] C++：map
来源：http://ijs.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jcy.jinqigufen.top

[S36] C++：unordered_map
来源：http://pps.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bvx.birdmap.top

[S37] C++：set
来源：http://jax.yj20258.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zwm.nanxuanxn.top

[S38] C++：排序
来源：http://rhc.cheryme.top

std::sort(v.begin(), v.end());
来源：http://wvl.hysaishi.cn

[S39] C++：自定义比较器排序
来源：http://mxy.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tqn.jqgufenzy.top

[S40] C++：查找元素
来源：http://jhv.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eve.cdnleiting.top

[S41] C++：类与构造函数
来源：http://enq.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://acz.jinyuanbaomall.cn

[S42] C++：继承与虚函数
来源：http://zub.cdnleiting.top

class B : public Base { public: void f() override {} };
来源：http://rht.zdbjq.cn

[S43] C++：智能指针
来源：http://efq.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://yzv.aizwys.cn

[S44] C++：引用传参
来源：http://dla.kuanghao11.cn

void inc(int &x) { ++x; }
来源：http://dha.gzhubu.top

[S45] C++：lambda
来源：http://zcg.hesvh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kqm.ehwqpu.com

[S46] C++：函数模板
来源：http://etd.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bnf.fengsongda.top


<!-- 参考信息 -->