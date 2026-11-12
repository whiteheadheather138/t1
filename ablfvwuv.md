代发 wailian999

[Q86] 读取 JSON 字段
来源：http://sjz.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dbg.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://bfl.0kj1m.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hhi.fktsv.cn

[Q88] 行转列（条件聚合）
来源：http://dkp.xuanzx.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fyj.iojbl.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uik.ppjwa.cn

[Q89] 判断表是否存在
来源：http://wal.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cgq.jianghu66.top

[Q90] 生成序号列
来源：http://kpw.epnwcf.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qlv.shanyushiyangtech.top

================================================================================
来源：http://sgt.meibo888.top

R. Bash 专题
来源：http://gbk.cucudq.cn

================================================================================
来源：http://fhq.hysaishi.cn

[R01] shebang 与严格模式
来源：http://jmm.9152youxi.cn

#!/usr/bin/env bash
来源：http://bvy.9152youxi.cn

set -euo pipefail
来源：http://fgx.ivvv.top

[R02] 变量赋值与使用
来源：http://prz.hammf.cn

name="Tom"; echo "$name"
来源：http://rbm.bjfxy.top

[R03] 只读变量
来源：http://drs.guannengcc.top

readonly PI=3.14
来源：http://srm.ivvv.top

[R04] 位置参数
来源：http://zwu.yfazqb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://biq.pengpengdd.cyou

[R05] 参数默认值
来源：http://jbq.hammf.cn

name="${1:-default}"
来源：http://psc.tianlin.xyz

[R06] 判断命令是否存在
来源：http://qwj.hnqzz.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rdp.aizwys.cn

[R07] if 判断文件
来源：http://crr.daxiang520.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xls.wangdashe.top

[R08] 数值比较
来源：http://sdk.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rxm.yuanzhike.top

[R09] 字符串比较
来源：http://oww.52xcode.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wwj.andypj.xyz

[R10] 正则匹配
来源：http://wvf.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ixw.snrcjt.cn

[R11] case 多分支
来源：http://gqx.iojbl.cn

case "$1" in
来源：http://mkc.wangshuangyany.cn

start) echo "启动" ;;
来源：http://wqf.dianchejie.cn

stop)  echo "停止" ;;
来源：http://jfr.ydzc1.top

*)     echo "未知命令" ;;
来源：http://nbc.gotoacloud.top

esac
来源：http://cfb.xuetiantiany.cn

[R12] for 遍历文件
来源：http://zba.yj20258888.top

for f in *.txt; do echo "$f"; done
来源：http://clh.316326.xyz

[R13] for 计数循环
来源：http://wfl.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://vgb.zhengqikj.top

[R14] C 风格 for
来源：http://jxh.52xcode.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://asz.daxiang520.top

[R15] while 逐行读文件
来源：http://rwk.zdbjq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jft.tanke756.top

[R16] until 等待条件
来源：http://gsd.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jcs.xylfe.cn

[R17] 数组定义与取值
来源：http://qvf.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qcu.meibo888.top

[R18] 遍历数组
来源：http://wra.xuanzx.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://anu.jlsjyb.cn

[R19] 数组长度
来源：http://wkm.chenlongwang.top

echo "${#arr[@]}"
来源：http://kxv.yangfankeji.com

[R20] 关联数组（字典）
来源：http://qox.yj20258.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xzi.guowangkeji.top

[R21] 字符串长度
来源：http://awy.fzhhl.top

echo "${#s}"
来源：http://ded.yuanzhike.top

[R22] 截取子串
来源：http://mxl.ybcxt.top

echo "${s:0:5}"
来源：http://qkg.pycfn.com

[R23] 字符串替换
来源：http://ytc.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kch.mhx1999.top

[R24] 大小写转换
来源：http://amq.iojbl.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ujv.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://nig.shangyingyoupin.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kmy.sweek.top

[R26] 命令替换
来源：http://vxp.yanxiufei.cn

now=$(date +%F); echo "$now"
来源：http://qwq.epnwcf.com

[R27] 算术展开
来源：http://kgm.jinghuilouyu.cn

echo $((1 + 2 * 3))
来源：http://xor.haohaochexian.top

[R28] 浮点运算
来源：http://lve.shuidangran.top

echo "scale=2; 10/3" | bc
来源：http://akf.zhixingplan.top

[R29] 定义函数
来源：http://xta.daria6918.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tin.wangshuangyany.cn

[R30] 函数返回状态码
来源：http://zun.shuidangran.top

f() { return 0; }; f || echo "失败了"
来源：http://osq.0kj1m.cn

[R31] 局部变量
来源：http://mlz.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://wsb.bjfxy.top

[R32] 参数个数校验
来源：http://qyk.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xfy.zycfv.cn

[R33] 捕获错误并提示行号
来源：http://gkw.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uva.ydjk.org.cn

[R34] 退出时清理
来源：http://ake.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://gxy.zdbjq.cn

[R35] 后台执行并等待
来源：http://oao.sxryk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kpo.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://hfu.sjlbkw.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kpe.tarul.cn

[R37] 把输出赋给变量
来源：http://ybh.hysaishi.cn

files=$(ls -1)
来源：http://ffm.yuxming.cn

[R38] 管道串联
来源：http://ned.xinyue.icu

cat a.txt | grep -i error | wc -l
来源：http://hqz.nanxinkj.top

[R39] 重定向标准输出与错误
来源：http://wbz.gaohongyu789.top

cmd > out.log 2>&1
来源：http://vin.hywenlv.cn

[R40] 追加写日志
来源：http://gol.fengsongda.top

echo "log" >> out.log
来源：http://vhq.ybcxt.top

[R41] 丢弃输出
来源：http://jad.hnqzz.top

cmd >/dev/null 2>&1
来源：http://iyu.wangdashe.top

[R42] 输入重定向
来源：http://piu.sjlbkw.cn

wc -l < a.txt
来源：http://hdj.hesvh.cn

[R43] 按名字查找文件
来源：http://uno.sweek.top

find . -name "*.log" -type f
来源：http://sdf.vehdjk.com

[R44] 按修改时间查找
来源：http://crl.yanxiufei.cn

find . -mtime -7 -type f
来源：http://ikx.chenjidiqi.icu

[R45] 批量删除
来源：http://vvw.jqgfzy.top

find . -name "*.tmp" -delete
来源：http://oxj.gaohongyu789.top

[R46] 递归替换文件内容
来源：http://obz.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hea.daria6918.cn

[R47] sed 单行替换
来源：http://udt.nanxuanxn.top

sed -i 's/foo/bar/g' a.txt
来源：http://tjh.dianchejie.cn

[R48] awk 取指定列
来源：http://rzy.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://lqg.ehwqpu.com

[R49] awk 带条件
来源：http://gpi.sxryk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aet.jyoumei.cn

[R50] awk 求和
来源：http://hbs.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vlm.vqdsnc.cn

[R51] 排序去重取前几
来源：http://jul.tarul.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eof.jyoumei.cn

[R52] 统计行数
来源：http://cgp.fzhhl.top

wc -l a.txt
来源：http://xjw.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://haf.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hpf.dashuyun.cn

[R54] 比较两个文件
来源：http://fon.zhaomingkeji.xyz

diff a.txt b.txt
来源：http://ppd.ivvv.top

[R55] 压缩与解压
来源：http://efv.hongshengwenyu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yth.cheryme.top

[R56] 远程拷贝
来源：http://vsz.52xcode.cn

scp file user@host:/path/
来源：http://vdv.yangfankeji.com

[R57] 远程执行命令
来源：http://scm.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://dlf.shanyushiyangtech.top

[R58] 下载文件
来源：http://dcj.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://owx.zhixingplan.top

[R59] 发 POST JSON
来源：http://zwh.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bqy.cdnleiting.top

[R60] 只看 HTTP 状态码
来源：http://gkh.kuanghao11.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kgz.tarul.cn

[R61] 磁盘占用
来源：http://jwj.dianchejie.cn

df -h;  du -sh *
来源：http://bkv.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://ikd.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://aqv.yuxming.cn

[R63] 内存与进程
来源：http://fyl.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://oom.hfpthk.cn

[R64] 结束进程
来源：http://nqw.yj202588.top

kill -9 $(pgrep -f app.py)
来源：http://ivk.xingfuxueyuan.xyz

[R65] 查看端口占用
来源：http://ouq.hfpthk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pyf.cheryme.top

[R66] 定时任务
来源：http://gra.sxryk.cn

crontab -e;  crontab -l
来源：http://rky.ivvv.top

[R67] 生成随机十六进制串
来源：http://foh.bjfxy.top

openssl rand -hex 16
来源：http://pyw.gaohongyu789.top

[R68] 计算文件校验值
来源：http://fua.shzxlz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pmy.ybcxt.top

[R69] 生成随机密码
来源：http://lce.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://gnm.xziqi.cn

[R70] 时间戳与互转
来源：http://gks.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://xak.wangdashe.top

[R71] 日期格式化
来源：http://cur.birdmap.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://chj.jinqigufen.top

[R72] 等待端口就绪
来源：http://mlf.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oqm.vehdjk.com

[R73] 分割大日志
来源：http://ryj.ydzc1.top

split -l 1000 big.log part_
来源：http://mpe.hesvh.cn

[R74] 批量重命名
来源：http://mgn.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oxj.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://xuc.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://psu.dashuyun.cn

[R76] 使用临时文件
来源：http://isq.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pgq.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://brb.havefunace.top

read -rp "请输入: " ans
来源：http://fbw.52xcode.cn

[R78] 交互式菜单
来源：http://gpe.guowangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nkr.guannengcc.top

[R79] 解析命令行选项
来源：http://zrd.dianchejie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://itr.hammf.cn

[R80] 查看脚本执行耗时
来源：http://rki.haohaochexian.top

time ./run.sh
来源：http://fuh.wangdashe.top

================================================================================
来源：http://xom.iojbl.cn

S. C / C++ 专题
来源：http://mdw.yangfankeji.com

================================================================================
来源：http://akb.xinyue.icu

[S01] C：Hello World
来源：http://gcx.cucudq.cn

#include <stdio.h>
来源：http://kyt.xinyue.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://qxs.yongpay.top

[S02] C：变量与格式化输出
来源：http://kik.hywenlv.cn

int a = 10; printf("%d\n", a);
来源：http://hod.pycfn.com

[S03] C：读入整数
来源：http://tkw.shzxlz.cn

int x; scanf("%d", &x);
来源：http://qjg.0kj1m.cn

[S04] C：字符串复制
来源：http://djg.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mdd.aizwys.cn

[S05] C：字符串长度
来源：http://ygx.jinyuanbaomall.cn

strlen(s)
来源：http://qno.yj202588.top

[S06] C：字符串比较
来源：http://hyc.cashguo.top

strcmp(a, b) == 0
来源：http://yci.yfazqb.com

[S07] C：数组遍历求和
来源：http://peo.jyoumei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://htn.havefunace.top

[S08] C：动态内存分配与释放
来源：http://utz.guannengcc.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ekm.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://iil.nanxinkj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rdn.hfpthk.cn

[S10] C：指针与解引用
来源：http://tod.fzhhl.top

int *p = &a;  *p = 5;
来源：http://tft.jinqigufen.top

[S11] C：逐行读文件
来源：http://mlz.xziqi.cn

FILE *f = fopen("a.txt", "r");
来源：http://fri.jyoumei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dvp.andypj.xyz

fclose(f);
来源：http://nuv.shangyingyoupin.top

[S12] C：写文件
来源：http://qiz.shanyushiyangtech.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ipd.gogol.net.cn

[S13] C：宏定义
来源：http://wml.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fho.pycfn.com

[S14] C：枚举
来源：http://jvc.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://qfd.sweek.top

[S15] C：类型转换
来源：http://rxb.aizwys.cn

(double) a / b
来源：http://qxo.yuxming.cn

[S16] C：位操作置位
来源：http://ora.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://iho.vehdjk.com

[S17] C：安全拼接字符串
来源：http://iwf.chenjidiqi.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ehk.yfazqb.com

[S18] C：命令行参数
来源：http://xtt.snrcjt.cn

int main(int argc, char **argv)
来源：http://ggr.yonumen.top

[S19] C：快速排序
来源：http://ccm.tian-w.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bkq.yuxming.cn

[S20] C：二分查找
来源：http://tlr.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uri.ybcxt.top

[S21] C：字符类别判断
来源：http://jrp.epnwcf.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wju.shangyingyoupin.top

[S22] C：字符串转数字
来源：http://dmd.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://axb.quarkkingdee.top

[S23] C：随机数
来源：http://agc.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xnl.0kj1m.cn

[S24] C：获取本地时间
来源：http://ejp.vqdsnc.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vdo.cucudq.cn

[S25] C：内存拷贝
来源：http://mgz.sxryk.cn

memcpy(dst, src, n);
来源：http://ysz.zdqjudy.top

[S26] C：内存清零
来源：http://mzi.chenlongwang.top

memset(a, 0, sizeof a);
来源：http://ddp.hnqzz.top

[S27] C：定义常量
来源：http://mpd.pengpengdd.cyou

const double PI = 3.14159;
来源：http://fvp.jiagoushi.top

[S28] C：静态变量
来源：http://jph.ivvv.top

static int counter = 0;
来源：http://ouz.shuidangran.top

[S29] C：变参函数
来源：http://xlm.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eqa.ivvv.top

[S30] C：头文件保护
来源：http://ubs.birdmap.top

#ifndef X_H
来源：http://mwr.sxryk.cn

#define X_H
来源：http://hsg.nanxuanxn.top

#endif
来源：http://rcy.fzhhl.top

[S31] C++：Hello World
来源：http://ted.jiagoushi.top

#include <iostream>
来源：http://qxt.zhengqikj.top

int main() { std::cout << "Hello\n"; }
来源：http://lxl.yvedp.cn

[S32] C++：字符串
来源：http://viw.wangshuangyany.cn

std::string s = "hi";  s += "!";
来源：http://qfc.wangdashe.top

[S33] C++：vector 增删
来源：http://qzf.uphjek.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nsa.52xcode.cn

[S34] C++：遍历 vector
来源：http://ztf.feifeiyinyue.top

for (auto &x : v) { std::cout << x; }
来源：http://fit.c1oappe.top

[S35] C++：map
来源：http://cky.9152youxi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kzn.ydzc1.top

[S36] C++：unordered_map
来源：http://xhl.fengsongda.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fpe.smart0.xyz

[S37] C++：set
来源：http://qfd.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bkm.yfazqb.com

[S38] C++：排序
来源：http://glf.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://ovz.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://nuw.vqdsnc.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oug.chenzaomai.com

[S40] C++：查找元素
来源：http://fsi.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qjz.c1oappe.top

[S41] C++：类与构造函数
来源：http://qgh.fzhhl.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vif.guowangkeji.top

[S42] C++：继承与虚函数
来源：http://zpu.yueranfly.top

class B : public Base { public: void f() override {} };
来源：http://fdx.tarul.cn

[S43] C++：智能指针
来源：http://eqm.zhengqikj.top

auto p = std::make_unique<int>(5);
来源：http://tfv.jinyuanbaomall.cn

[S44] C++：引用传参
来源：http://rmb.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://dyh.kuanghao11.cn

[S45] C++：lambda
来源：http://tox.ehwqpu.com

auto add = [](int a, int b) { return a + b; };
来源：http://boo.jlsjyb.cn

[S46] C++：函数模板
来源：http://qdz.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ksh.zdqjudy.top

[S47] C++：结构化绑定遍历
来源：http://ugq.xziqi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zqj.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://goy.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://hfm.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://rvw.snrcjt.cn

[S49] C++：写文件
来源：http://vod.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ned.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://tbv.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rcm.birdmap.top

[S51] C++：显式类型转换
来源：http://wis.jinyuanbaomall.cn

static_cast<double>(a) / b
来源：http://ybv.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://lwj.kuanghao11.cn

int size() const noexcept { return n_; }
来源：http://ugh.yanxiufei.cn

[S53] C++：移动语义
来源：http://ioj.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://xsq.xuanzx.com

[S54] C++：异常处理
来源：http://egw.zhiwuduotai.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uza.cheryme.top

[S55] C++：结构化绑定
来源：http://dsr.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://cyb.bjfxy.top

[S56] C++：optional
来源：http://zip.9152youxi.cn


<!-- 参考信息 -->