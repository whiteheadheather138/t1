代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://jqp.fengsongda.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xna.zhijiandao.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uzg.52xcode.cn

[Q89] 判断表是否存在
来源：http://ftb.wangdashe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wyt.316326.xyz

[Q90] 生成序号列
来源：http://qwo.chenzaomai.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bin.yangfankeji.com

================================================================================
来源：http://fgf.guannengcc.top

R. Bash 专题
来源：http://yei.hesvh.cn

================================================================================
来源：http://qfr.bjfxy.top

[R01] shebang 与严格模式
来源：http://wbt.yj20258.top

#!/usr/bin/env bash
来源：http://ehc.dashuyun.cn

set -euo pipefail
来源：http://mun.hywenlv.cn

[R02] 变量赋值与使用
来源：http://lji.wangdashe.top

name="Tom"; echo "$name"
来源：http://keo.sysykeji.top

[R03] 只读变量
来源：http://gtj.hysaishi.cn

readonly PI=3.14
来源：http://rte.chenzaomai.com

[R04] 位置参数
来源：http://lvt.shangyingyoupin.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ruw.feifeiyinyue.top

[R05] 参数默认值
来源：http://dbc.52xcode.cn

name="${1:-default}"
来源：http://yrt.havefunace.top

[R06] 判断命令是否存在
来源：http://cov.tarul.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hrr.yongpay.top

[R07] if 判断文件
来源：http://sov.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lee.hammf.cn

[R08] 数值比较
来源：http://ahe.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://cdh.zhoulong.xyz

[R09] 字符串比较
来源：http://bqj.yj20258.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://iwf.316326.xyz

[R10] 正则匹配
来源：http://bjm.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://apf.zhaomingkeji.xyz

[R11] case 多分支
来源：http://bpm.hnqzz.top

case "$1" in
来源：http://cbg.gzhubu.top

start) echo "启动" ;;
来源：http://cea.chenlongwang.top

stop)  echo "停止" ;;
来源：http://xft.52xcode.cn

*)     echo "未知命令" ;;
来源：http://rnf.iojbl.cn

esac
来源：http://iyi.yj20258.top

[R12] for 遍历文件
来源：http://zqg.jinqigfzy.top

for f in *.txt; do echo "$f"; done
来源：http://qqj.fanxiaobao.xyz

[R13] for 计数循环
来源：http://kiv.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://idl.jinqigufen.top

[R14] C 风格 for
来源：http://idy.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ajc.meibo888.top

[R15] while 逐行读文件
来源：http://ihg.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xob.zhengqikj.top

[R16] until 等待条件
来源：http://scq.nanxuanxn.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lhn.hfpthk.cn

[R17] 数组定义与取值
来源：http://wyi.jianghu66.top

arr=(a b c); echo "${arr[0]}"
来源：http://eub.yongpay.top

[R18] 遍历数组
来源：http://sfj.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ypc.hfpthk.cn

[R19] 数组长度
来源：http://buo.cashguo.top

echo "${#arr[@]}"
来源：http://rwm.hnxiangtu.top

[R20] 关联数组（字典）
来源：http://xvn.jinyuanbaomall.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rhi.hongshengwenyu.top

[R21] 字符串长度
来源：http://ezx.gzhubu.top

echo "${#s}"
来源：http://vqz.yuxming.cn

[R22] 截取子串
来源：http://ivq.birdmap.top

echo "${s:0:5}"
来源：http://nem.52xcode.cn

[R23] 字符串替换
来源：http://gan.guannengcc.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oru.andypj.xyz

[R24] 大小写转换
来源：http://dac.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://xuz.quarkkingdee.top

[R25] 去后缀 / 去前缀
来源：http://qys.smart0.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://afo.ywan-chungtsiang.top

[R26] 命令替换
来源：http://uco.cashguo.top

now=$(date +%F); echo "$now"
来源：http://for.tarul.cn

[R27] 算术展开
来源：http://tqh.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://opq.mhx1999.top

[R28] 浮点运算
来源：http://fbe.ctjpmb.com

echo "scale=2; 10/3" | bc
来源：http://yij.hongshengwenyu.top

[R29] 定义函数
来源：http://arw.gotoacloud.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aqf.ywan-chungtsiang.top

[R30] 函数返回状态码
来源：http://ouu.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://yeq.yfazqb.com

[R31] 局部变量
来源：http://nwj.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://nfd.hywenlv.cn

[R32] 参数个数校验
来源：http://fom.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://llj.yuanzhike.top

[R33] 捕获错误并提示行号
来源：http://tna.fktsv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fpu.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://aeu.yangfankeji.com

trap 'rm -f "$tmp"' EXIT
来源：http://yvz.jinqigfzy.top

[R35] 后台执行并等待
来源：http://zzo.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://iax.cheryme.top

[R36] 并发执行多个任务
来源：http://esg.dianchejie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dzv.yonumen.top

[R37] 把输出赋给变量
来源：http://dvu.sxryk.cn

files=$(ls -1)
来源：http://awg.jyoumei.cn

[R38] 管道串联
来源：http://mns.cheryme.top

cat a.txt | grep -i error | wc -l
来源：http://hjl.ydjk.org.cn

[R39] 重定向标准输出与错误
来源：http://mkb.dashuyun.cn

cmd > out.log 2>&1
来源：http://jwx.meibo888.top

[R40] 追加写日志
来源：http://ysm.hfpthk.cn

echo "log" >> out.log
来源：http://usr.feifeiyinyue.top

[R41] 丢弃输出
来源：http://rnh.fengsongda.top

cmd >/dev/null 2>&1
来源：http://tes.hammf.cn

[R42] 输入重定向
来源：http://gzh.gzhubu.top

wc -l < a.txt
来源：http://eon.yvedp.cn

[R43] 按名字查找文件
来源：http://kox.xingfuxueyuan.xyz

find . -name "*.log" -type f
来源：http://urv.fktsv.cn

[R44] 按修改时间查找
来源：http://qqe.jinghuilouyu.cn

find . -mtime -7 -type f
来源：http://hdu.jinqigufen.top

[R45] 批量删除
来源：http://rvp.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://trx.hfpthk.cn

[R46] 递归替换文件内容
来源：http://bwg.xinyue.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://beb.hywenlv.cn

[R47] sed 单行替换
来源：http://vrg.aizwys.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gcp.yanxiufei.cn

[R48] awk 取指定列
来源：http://xwl.mhx1999.top

awk '{print $1, $3}' a.txt
来源：http://qmw.yuxming.cn

[R49] awk 带条件
来源：http://ief.vqdsnc.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://upb.havefunace.top

[R50] awk 求和
来源：http://wzo.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://hxl.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://ycx.cashguo.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jtw.tian-w.cn

[R52] 统计行数
来源：http://fhf.ctjpmb.com

wc -l a.txt
来源：http://dox.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://beh.wangdashe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kgn.jinyuanbaomall.cn

[R54] 比较两个文件
来源：http://ivt.zhijiandao.cn

diff a.txt b.txt
来源：http://gle.snrcjt.cn

[R55] 压缩与解压
来源：http://uoe.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wor.ydjk.org.cn

[R56] 远程拷贝
来源：http://kqb.jinghuilouyu.cn

scp file user@host:/path/
来源：http://cgy.nanxuanxn.top

[R57] 远程执行命令
来源：http://gxx.zhengqikj.top

ssh user@host 'uptime'
来源：http://jfq.hcnkem.com

[R58] 下载文件
来源：http://sjn.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://avt.guowangkeji.top

[R59] 发 POST JSON
来源：http://bqe.mhx1999.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bwn.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://txn.zhixingplan.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uiz.uphjek.com

[R61] 磁盘占用
来源：http://sas.zhixingplan.top

df -h;  du -sh *
来源：http://dju.yj20258888.top

[R62] 找最占空间的文件
来源：http://ccx.birdmap.top

du -ah . | sort -rh | head -10
来源：http://qaa.dashuyun.cn

[R63] 内存与进程
来源：http://jhc.zhiwuduotai.top

free -h;  ps aux | grep nginx
来源：http://goo.yj20258888.top

[R64] 结束进程
来源：http://vee.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://pua.vehdjk.com

[R65] 查看端口占用
来源：http://ivu.gotoacloud.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wgb.hysaishi.cn

[R66] 定时任务
来源：http://dnz.svipenyu.cn

crontab -e;  crontab -l
来源：http://pwq.xuetiantiany.cn

[R67] 生成随机十六进制串
来源：http://feg.shanyushiyangtech.top

openssl rand -hex 16
来源：http://atn.vqdsnc.cn

[R68] 计算文件校验值
来源：http://jco.sxryk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mhl.bbcook.cn

[R69] 生成随机密码
来源：http://rgr.zhijiandao.cn

head -c 16 /dev/urandom | base64
来源：http://mpz.tanke756.top

[R70] 时间戳与互转
来源：http://tcg.52xcode.cn

date +%s;  date -d @1700000000
来源：http://rib.hcnkem.com

[R71] 日期格式化
来源：http://wgq.wangdashe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nsy.ydjk.org.cn

[R72] 等待端口就绪
来源：http://jgj.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rwp.ctjpmb.com

[R73] 分割大日志
来源：http://hfi.epnwcf.com

split -l 1000 big.log part_
来源：http://irv.yueranfly.top

[R74] 批量重命名
来源：http://pbk.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vdp.bbcook.cn

[R75] 导出环境变量
来源：http://nue.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://isf.zhixingplan.top

[R76] 使用临时文件
来源：http://niu.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fjf.aizwys.cn

[R77] 读取用户输入
来源：http://day.mhx1999.top

read -rp "请输入: " ans
来源：http://tjd.gaohongyu789.top

[R78] 交互式菜单
来源：http://hrj.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pmn.guannengcc.top

[R79] 解析命令行选项
来源：http://gwf.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lcj.ybcxt.top

[R80] 查看脚本执行耗时
来源：http://bbo.mhx1999.top

time ./run.sh
来源：http://kar.aibaodan.cn

================================================================================
来源：http://ysc.zhengqikj.top

S. C / C++ 专题
来源：http://qhl.xuanzx.com

================================================================================
来源：http://jzx.hywenlv.cn

[S01] C：Hello World
来源：http://fkj.tian-w.cn

#include <stdio.h>
来源：http://qow.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qze.hammf.cn

[S02] C：变量与格式化输出
来源：http://agr.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://xet.yonumen.top

[S03] C：读入整数
来源：http://lms.jiagoushi.top

int x; scanf("%d", &x);
来源：http://ixt.ehwqpu.com

[S04] C：字符串复制
来源：http://nrc.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://txs.ehwqpu.com

[S05] C：字符串长度
来源：http://sqx.yj20258888.top

strlen(s)
来源：http://duz.bbcook.cn

[S06] C：字符串比较
来源：http://pcb.hnxiangtu.top

strcmp(a, b) == 0
来源：http://spq.yvedp.cn

[S07] C：数组遍历求和
来源：http://pie.jlsjyb.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cdq.jiagoushi.top

[S08] C：动态内存分配与释放
来源：http://rpj.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fhj.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://ndt.sufxvd.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iin.bbcook.cn

[S10] C：指针与解引用
来源：http://xvs.svipenyu.cn

int *p = &a;  *p = 5;
来源：http://lsn.gzhubu.top

[S11] C：逐行读文件
来源：http://dpu.yj20258888.top

FILE *f = fopen("a.txt", "r");
来源：http://qdo.gogol.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xrn.zdqjudy.top

fclose(f);
来源：http://wja.zhongyouzk.top

[S12] C：写文件
来源：http://qhw.jqgufenzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://feg.ydzc1.top

[S13] C：宏定义
来源：http://sym.xziqi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://osd.haohaochexian.top

[S14] C：枚举
来源：http://scz.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://kyl.jinqigfzy.top

[S15] C：类型转换
来源：http://wem.redwolf501.top

(double) a / b
来源：http://htl.ydjk.org.cn

[S16] C：位操作置位
来源：http://jqo.aibaodan.cn

x |= (1 << 3);
来源：http://utn.c1oappe.top

[S17] C：安全拼接字符串
来源：http://lbp.jqgfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bmt.ybcxt.top

[S18] C：命令行参数
来源：http://zdn.pengpengdd.cyou

int main(int argc, char **argv)
来源：http://heg.c1oappe.top

[S19] C：快速排序
来源：http://avu.316326.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://wmv.yangfankeji.com

[S20] C：二分查找
来源：http://zce.ydzc1.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tax.chenzaomai.com

[S21] C：字符类别判断
来源：http://ejy.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://alf.jianghu66.top

[S22] C：字符串转数字
来源：http://avx.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://klv.sweek.top

[S23] C：随机数
来源：http://ria.tian-w.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://row.hysaishi.cn

[S24] C：获取本地时间
来源：http://ocd.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dzl.jinqigufen.top

[S25] C：内存拷贝
来源：http://zyw.daxiang520.top

memcpy(dst, src, n);
来源：http://qre.zhengqikj.top

[S26] C：内存清零
来源：http://bep.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://zah.zhaomingkeji.xyz

[S27] C：定义常量
来源：http://vxy.feifeiyinyue.top

const double PI = 3.14159;
来源：http://ajk.xuetiantiany.cn

[S28] C：静态变量
来源：http://xvi.ydjk.org.cn

static int counter = 0;
来源：http://qtz.guowangkeji.top

[S29] C：变参函数
来源：http://dva.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pox.xuetiantiany.cn

[S30] C：头文件保护
来源：http://ltk.yuxming.cn

#ifndef X_H
来源：http://pcq.tianlin.xyz

#define X_H
来源：http://lgb.andypj.xyz

#endif
来源：http://quj.jinghuilouyu.cn

[S31] C++：Hello World
来源：http://wev.dashuyun.cn

#include <iostream>
来源：http://tuz.jianghu66.top

int main() { std::cout << "Hello\n"; }
来源：http://htv.jqgfzy.top

[S32] C++：字符串
来源：http://oyu.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://iol.9152youxi.cn

[S33] C++：vector 增删
来源：http://fwh.pycfn.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oox.meibo888.top

[S34] C++：遍历 vector
来源：http://yzp.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://kiy.xuetiantiany.cn

[S35] C++：map
来源：http://lsu.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lft.chenlongwang.top

[S36] C++：unordered_map
来源：http://inw.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://egu.tianlin.xyz

[S37] C++：set
来源：http://itl.fzhhl.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lln.chenzaomai.com

[S38] C++：排序
来源：http://bkc.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://swl.zhoulong.xyz

[S39] C++：自定义比较器排序
来源：http://onf.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gyb.fanxiaobao.xyz

[S40] C++：查找元素
来源：http://fxd.yuanzhike.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hdc.svipenyu.cn

[S41] C++：类与构造函数
来源：http://tnc.zhijiandao.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://krc.sxryk.cn

[S42] C++：继承与虚函数
来源：http://sfa.ppjwa.cn

class B : public Base { public: void f() override {} };
来源：http://lyv.cashguo.top

[S43] C++：智能指针
来源：http://cvj.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://whv.shangyingyoupin.top

[S44] C++：引用传参
来源：http://sdw.epnwcf.com

void inc(int &x) { ++x; }
来源：http://vdn.yj20258.top

[S45] C++：lambda
来源：http://lkn.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://aqw.gzhubu.top

[S46] C++：函数模板
来源：http://yxi.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wjs.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://gnb.ydjk.org.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://byb.pycfn.com

[S48] C++：逐行读文件
来源：http://cmp.sweek.top

std::ifstream in("a.txt");  std::string line;
来源：http://hpl.jinqigfzy.top

while (std::getline(in, line)) { }
来源：http://cwi.daxiang520.top

[S49] C++：写文件
来源：http://rck.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iif.jiagoushi.top

[S50] C++：格式化数字
来源：http://jhh.zhixingplan.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nyy.tanke756.top

[S51] C++：显式类型转换
来源：http://rxs.redwolf501.top

static_cast<double>(a) / b
来源：http://fwe.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://sku.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://qwe.yueranfly.top

[S53] C++：移动语义
来源：http://hym.havefunace.top

std::vector<int> w = std::move(v);
来源：http://rcy.gotoacloud.top

[S54] C++：异常处理
来源：http://hdu.yvedp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nui.jqgfzy.top

[S55] C++：结构化绑定
来源：http://scs.yfazqb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://qwu.epnwcf.com

[S56] C++：optional
来源：http://ywp.ppjwa.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jhg.nwbrower.top

[S57] C++：编译期常量
来源：http://zyh.nwbrower.top

constexpr int N = 10;
来源：http://dut.cucudq.cn

[S58] C++：命名空间
来源：http://ssr.dianchejie.cn


<!-- 参考信息 -->