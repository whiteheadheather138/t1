代发 wailian999

[Q86] 读取 JSON 字段
来源：http://ynl.yuanzhike.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dap.0kj1m.cn

[Q87] JSON 字段做条件
来源：http://zcp.tanke756.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://esr.hcnkem.com

[Q88] 行转列（条件聚合）
来源：http://fji.svipenyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rkr.jqgfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zkw.ydjk.org.cn

[Q89] 判断表是否存在
来源：http://fkb.aizwys.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://msw.hysaishi.cn

[Q90] 生成序号列
来源：http://ihs.hnxiangtu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ecc.zdbjq.cn

================================================================================
来源：http://xvm.hcnkem.com

R. Bash 专题
来源：http://dcp.jinqigufen.top

================================================================================
来源：http://fgg.hongshengwenyu.top

[R01] shebang 与严格模式
来源：http://eef.andypj.xyz

#!/usr/bin/env bash
来源：http://new.uphjek.com

set -euo pipefail
来源：http://zzp.fehbvm.com

[R02] 变量赋值与使用
来源：http://nvp.yongpay.top

name="Tom"; echo "$name"
来源：http://csp.ctjpmb.com

[R03] 只读变量
来源：http://omq.meibo888.top

readonly PI=3.14
来源：http://sql.jinyuanbaomall.cn

[R04] 位置参数
来源：http://cif.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dgv.guowangkeji.top

[R05] 参数默认值
来源：http://qqs.vehdjk.com

name="${1:-default}"
来源：http://rkv.kuanghao11.cn

[R06] 判断命令是否存在
来源：http://ywa.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aje.zhengqikj.top

[R07] if 判断文件
来源：http://qcs.jinyuanbaomall.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://clg.xziqi.cn

[R08] 数值比较
来源：http://sic.jinqigfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://yes.nwbrower.top

[R09] 字符串比较
来源：http://gdo.quarkkingdee.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://puz.gotoacloud.top

[R10] 正则匹配
来源：http://ozs.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ugu.nanxinkj.top

[R11] case 多分支
来源：http://cif.ehwqpu.com

case "$1" in
来源：http://bah.gaohongyu789.top

start) echo "启动" ;;
来源：http://szg.cqqwz.cn

stop)  echo "停止" ;;
来源：http://bwl.shzxlz.cn

*)     echo "未知命令" ;;
来源：http://xby.zdbjq.cn

esac
来源：http://wyr.xuanzx.com

[R12] for 遍历文件
来源：http://yut.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://ujm.chenjidiqi.icu

[R13] for 计数循环
来源：http://dxh.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://qoy.chenlongwang.top

[R14] C 风格 for
来源：http://kof.jinqigfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://elr.ivvv.top

[R15] while 逐行读文件
来源：http://vrs.hesvh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://diu.zhiwuduotai.top

[R16] until 等待条件
来源：http://hcm.fanxiaobao.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ycw.smart0.xyz

[R17] 数组定义与取值
来源：http://llc.bbcook.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yri.chenlongwang.top

[R18] 遍历数组
来源：http://dpt.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://piv.birdmap.top

[R19] 数组长度
来源：http://eqk.ehwqpu.com

echo "${#arr[@]}"
来源：http://rod.ivvv.top

[R20] 关联数组（字典）
来源：http://yax.nanxuanxn.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wru.yj20258.top

[R21] 字符串长度
来源：http://qis.nwbrower.top

echo "${#s}"
来源：http://bzl.ehwqpu.com

[R22] 截取子串
来源：http://aew.cheryme.top

echo "${s:0:5}"
来源：http://ols.jqgufenzy.top

[R23] 字符串替换
来源：http://jsi.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://haz.ybcxt.top

[R24] 大小写转换
来源：http://mwe.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mjy.9152youxi.cn

[R25] 去后缀 / 去前缀
来源：http://jie.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ohw.sufxvd.cn

[R26] 命令替换
来源：http://cya.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://fel.hysaishi.cn

[R27] 算术展开
来源：http://fli.hnqzz.top

echo $((1 + 2 * 3))
来源：http://jfb.ybcxt.top

[R28] 浮点运算
来源：http://gfx.tarul.cn

echo "scale=2; 10/3" | bc
来源：http://zxh.birdmap.top

[R29] 定义函数
来源：http://yla.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ppo.sysykeji.top

[R30] 函数返回状态码
来源：http://gqd.dashuyun.cn

f() { return 0; }; f || echo "失败了"
来源：http://roa.jlsjyb.cn

[R31] 局部变量
来源：http://ilc.ctjpmb.com

f() { local x=1; echo "$x"; }
来源：http://woa.iojbl.cn

[R32] 参数个数校验
来源：http://asx.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vsn.yuanzhike.top

[R33] 捕获错误并提示行号
来源：http://vyo.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qvl.xziqi.cn

[R34] 退出时清理
来源：http://cig.epnwcf.com

trap 'rm -f "$tmp"' EXIT
来源：http://xrh.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://sym.jinqigufen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kzm.zhongyouzk.top

[R36] 并发执行多个任务
来源：http://kfm.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tbh.xylfe.cn

[R37] 把输出赋给变量
来源：http://qlq.yangfankeji.com

files=$(ls -1)
来源：http://vjh.cqqwz.cn

[R38] 管道串联
来源：http://ejg.chenzaomai.com

cat a.txt | grep -i error | wc -l
来源：http://vel.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://pah.zdbjq.cn

cmd > out.log 2>&1
来源：http://hmp.havefunace.top

[R40] 追加写日志
来源：http://oqp.quarkkingdee.top

echo "log" >> out.log
来源：http://yve.bjfxy.top

[R41] 丢弃输出
来源：http://dub.tarul.cn

cmd >/dev/null 2>&1
来源：http://svl.shanyushiyangtech.top

[R42] 输入重定向
来源：http://pjr.nanxuanxn.top

wc -l < a.txt
来源：http://gms.yonumen.top

[R43] 按名字查找文件
来源：http://djo.yonumen.top

find . -name "*.log" -type f
来源：http://sdc.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://cri.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://zuv.gotoacloud.top

[R45] 批量删除
来源：http://snk.xingfuxueyuan.xyz

find . -name "*.tmp" -delete
来源：http://vka.aizwys.cn

[R46] 递归替换文件内容
来源：http://naq.hnqzz.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lho.birdmap.top

[R47] sed 单行替换
来源：http://zpg.zdqjudy.top

sed -i 's/foo/bar/g' a.txt
来源：http://bnm.jinqigfzy.top

[R48] awk 取指定列
来源：http://mjb.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://dld.sysykeji.top

[R49] awk 带条件
来源：http://jes.xinyue.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://alo.bbcook.cn

[R50] awk 求和
来源：http://pky.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wya.jqgufenzy.top

[R51] 排序去重取前几
来源：http://ysf.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mzh.9152youxi.cn

[R52] 统计行数
来源：http://mee.zdbjq.cn

wc -l a.txt
来源：http://iro.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://tgz.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wqc.yvedp.cn

[R54] 比较两个文件
来源：http://mzm.ydjk.org.cn

diff a.txt b.txt
来源：http://dlz.zdqjudy.top

[R55] 压缩与解压
来源：http://wfk.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fbg.meibo888.top

[R56] 远程拷贝
来源：http://yds.yj202588.top

scp file user@host:/path/
来源：http://dvj.guowangkeji.top

[R57] 远程执行命令
来源：http://tuv.jinqigfzy.top

ssh user@host 'uptime'
来源：http://gpj.haohaochexian.top

[R58] 下载文件
来源：http://gyu.hcnkem.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vbc.hysaishi.cn

[R59] 发 POST JSON
来源：http://bte.tian-w.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kvv.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://qty.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xog.cashguo.top

[R61] 磁盘占用
来源：http://faz.nanxuanxn.top

df -h;  du -sh *
来源：http://lsi.snrcjt.cn

[R62] 找最占空间的文件
来源：http://ayu.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://jwj.vehdjk.com

[R63] 内存与进程
来源：http://nol.xuanzx.com

free -h;  ps aux | grep nginx
来源：http://pel.zhijiandao.cn

[R64] 结束进程
来源：http://eec.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://mxc.ehwqpu.com

[R65] 查看端口占用
来源：http://gan.guannengcc.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bei.gogol.net.cn

[R66] 定时任务
来源：http://jeh.chenzaomai.com

crontab -e;  crontab -l
来源：http://bbb.yj20258.top

[R67] 生成随机十六进制串
来源：http://oud.quarkkingdee.top

openssl rand -hex 16
来源：http://lim.fzhhl.top

[R68] 计算文件校验值
来源：http://smr.9152youxi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gel.xingfuxueyuan.xyz

[R69] 生成随机密码
来源：http://mlz.epnwcf.com

head -c 16 /dev/urandom | base64
来源：http://gem.ybcxt.top

[R70] 时间戳与互转
来源：http://aea.sufxvd.cn

date +%s;  date -d @1700000000
来源：http://xzs.shzxlz.cn

[R71] 日期格式化
来源：http://fhe.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bbv.zhijiandao.cn

[R72] 等待端口就绪
来源：http://pgc.shanyushiyangtech.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ish.ydjk.org.cn

[R73] 分割大日志
来源：http://blp.nanxinkj.top

split -l 1000 big.log part_
来源：http://sqy.nanxuanxn.top

[R74] 批量重命名
来源：http://rul.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://amp.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://rlv.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://ras.zhongyouzk.top

[R76] 使用临时文件
来源：http://yyx.guowangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gzp.yuanzhike.top

[R77] 读取用户输入
来源：http://wdt.ivvv.top

read -rp "请输入: " ans
来源：http://yzj.ehwqpu.com

[R78] 交互式菜单
来源：http://bjn.aizwys.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://onz.yanxiufei.cn

[R79] 解析命令行选项
来源：http://nhz.cheryme.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://enh.yongpay.top

[R80] 查看脚本执行耗时
来源：http://xsl.sjlbkw.cn

time ./run.sh
来源：http://vky.zhijiandao.cn

================================================================================
来源：http://wmp.jinghuilouyu.cn

S. C / C++ 专题
来源：http://ctp.hongshengwenyu.top

================================================================================
来源：http://fdg.yonumen.top

[S01] C：Hello World
来源：http://vvo.tian-w.cn

#include <stdio.h>
来源：http://rby.fktsv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lph.shuidangran.top

[S02] C：变量与格式化输出
来源：http://tzs.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://ceu.wangdashe.top

[S03] C：读入整数
来源：http://xem.kuanghao11.cn

int x; scanf("%d", &x);
来源：http://rja.yueranfly.top

[S04] C：字符串复制
来源：http://xwm.cqqwz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fpo.feifeiyinyue.top

[S05] C：字符串长度
来源：http://fuh.zdbjq.cn

strlen(s)
来源：http://pof.snrcjt.cn

[S06] C：字符串比较
来源：http://cus.pengpengdd.cyou

strcmp(a, b) == 0
来源：http://ndx.jyoumei.cn

[S07] C：数组遍历求和
来源：http://rjs.yuxming.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lyr.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://jef.hnqzz.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jab.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://nsk.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ldz.jiagoushi.top

[S10] C：指针与解引用
来源：http://fzr.yj202588.top

int *p = &a;  *p = 5;
来源：http://zkj.sysykeji.top

[S11] C：逐行读文件
来源：http://zkl.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://jnw.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vou.xylfe.cn

fclose(f);
来源：http://jgb.tarul.cn

[S12] C：写文件
来源：http://qcj.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wlz.tian-w.cn

[S13] C：宏定义
来源：http://rcn.nanxuanxn.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://urj.jlsjyb.cn

[S14] C：枚举
来源：http://zri.hammf.cn

enum Color { RED, GREEN, BLUE };
来源：http://nun.gaohongyu789.top

[S15] C：类型转换
来源：http://kzg.wangshuangyany.cn

(double) a / b
来源：http://ixd.bjfxy.top

[S16] C：位操作置位
来源：http://ipx.ivvv.top

x |= (1 << 3);
来源：http://sfg.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://khm.feifeiyinyue.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://snj.ppjwa.cn

[S18] C：命令行参数
来源：http://wxn.yvedp.cn

int main(int argc, char **argv)
来源：http://dzd.gaohongyu789.top

[S19] C：快速排序
来源：http://gwx.vehdjk.com

qsort(a, n, sizeof(int), cmp);
来源：http://sqs.ivvv.top

[S20] C：二分查找
来源：http://mvx.cashguo.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zey.gotoacloud.top

[S21] C：字符类别判断
来源：http://mbu.gaohongyu789.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cml.cashguo.top

[S22] C：字符串转数字
来源：http://jtf.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nul.yonumen.top

[S23] C：随机数
来源：http://jpy.jianghu66.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uly.ybcxt.top

[S24] C：获取本地时间
来源：http://xkr.cucudq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://npy.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://wvj.xziqi.cn

memcpy(dst, src, n);
来源：http://cbm.sjlbkw.cn

[S26] C：内存清零
来源：http://mvl.epnwcf.com

memset(a, 0, sizeof a);
来源：http://iry.nanxuanxn.top

[S27] C：定义常量
来源：http://twv.yueranfly.top

const double PI = 3.14159;
来源：http://zqx.vehdjk.com

[S28] C：静态变量
来源：http://eqa.jqgufenzy.top

static int counter = 0;
来源：http://mzb.zhoulong.xyz

[S29] C：变参函数
来源：http://hbk.yj20258888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://khr.sweek.top

[S30] C：头文件保护
来源：http://gfs.xuetiantiany.cn

#ifndef X_H
来源：http://xar.nanxinkj.top

#define X_H
来源：http://tev.ywan-chungtsiang.top

#endif
来源：http://ouk.kuanghao11.cn

[S31] C++：Hello World
来源：http://eci.fanxiaobao.xyz

#include <iostream>
来源：http://awy.fzhhl.top

int main() { std::cout << "Hello\n"; }
来源：http://koz.nanxuanxn.top

[S32] C++：字符串
来源：http://oee.fengsongda.top

std::string s = "hi";  s += "!";
来源：http://aym.ehwqpu.com

[S33] C++：vector 增删
来源：http://erh.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qom.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://ign.smart0.xyz

for (auto &x : v) { std::cout << x; }
来源：http://fez.zdbjq.cn

[S35] C++：map
来源：http://tdh.hammf.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pvm.fanxiaobao.xyz

[S36] C++：unordered_map
来源：http://iiq.wangdashe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dix.zycfv.cn

[S37] C++：set
来源：http://mor.zycfv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zbe.zhiwuduotai.top

[S38] C++：排序
来源：http://enq.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://pka.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://vpi.zdbjq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pyr.yj20258888.top

[S40] C++：查找元素
来源：http://hct.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ifw.cheryme.top

[S41] C++：类与构造函数
来源：http://wme.meibo888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wpw.hammf.cn

[S42] C++：继承与虚函数
来源：http://jmy.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://hin.cashguo.top

[S43] C++：智能指针
来源：http://cyh.sufxvd.cn

auto p = std::make_unique<int>(5);
来源：http://uvv.xylfe.cn

[S44] C++：引用传参
来源：http://tjj.zhoulong.xyz

void inc(int &x) { ++x; }
来源：http://nvd.bbcook.cn

[S45] C++：lambda
来源：http://rtb.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://jgj.yanxiufei.cn

[S46] C++：函数模板
来源：http://gkk.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qlp.fktsv.cn

[S47] C++：结构化绑定遍历
来源：http://lmo.sufxvd.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sdy.hywenlv.cn

[S48] C++：逐行读文件
来源：http://tjj.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://bge.fanxiaobao.xyz

while (std::getline(in, line)) { }
来源：http://ovv.wangshuangyany.cn

[S49] C++：写文件
来源：http://qdu.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vpl.dianchejie.cn

[S50] C++：格式化数字
来源：http://pln.0kj1m.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ghe.cqqwz.cn

[S51] C++：显式类型转换
来源：http://bzh.tanke756.top

static_cast<double>(a) / b
来源：http://nyu.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://jnw.gzhubu.top

int size() const noexcept { return n_; }
来源：http://rqd.cheryme.top

[S53] C++：移动语义
来源：http://sze.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://rid.yanxiufei.cn

[S54] C++：异常处理
来源：http://csd.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wcm.hfpthk.cn

[S55] C++：结构化绑定
来源：http://hji.yuanzhike.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jpn.jyoumei.cn

[S56] C++：optional
来源：http://hrx.yongpay.top


<!-- 参考信息 -->