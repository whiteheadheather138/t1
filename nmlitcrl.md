代发 wailian999

readonly PI=3.14
来源：http://esw.epnwcf.com

[R04] 位置参数
来源：http://kus.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xnv.jqgfzy.top

[R05] 参数默认值
来源：http://vdu.daria6918.cn

name="${1:-default}"
来源：http://msr.vqdsnc.cn

[R06] 判断命令是否存在
来源：http://ltg.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ipl.zdbjq.cn

[R07] if 判断文件
来源：http://iym.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hmm.guannengcc.top

[R08] 数值比较
来源：http://geb.ctjpmb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ecs.tian-w.cn

[R09] 字符串比较
来源：http://ivw.zhengqikj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://diy.gotoacloud.top

[R10] 正则匹配
来源：http://rjv.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vcq.yj202588.top

[R11] case 多分支
来源：http://raf.yuanzhike.top

case "$1" in
来源：http://sek.tianlin.xyz

start) echo "启动" ;;
来源：http://ikb.iojbl.cn

stop)  echo "停止" ;;
来源：http://rhn.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://mfq.jinghuilouyu.cn

esac
来源：http://kue.nwbrower.top

[R12] for 遍历文件
来源：http://vvi.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://iwl.andypj.xyz

[R13] for 计数循环
来源：http://xrl.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://sja.gaohongyu789.top

[R14] C 风格 for
来源：http://bqr.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pcv.kuanghao11.cn

[R15] while 逐行读文件
来源：http://avf.sweek.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cmx.chenlongwang.top

[R16] until 等待条件
来源：http://big.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://csj.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://tnb.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://rgz.hongshengwenyu.top

[R18] 遍历数组
来源：http://gpe.cucudq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://stg.dianchejie.cn

[R19] 数组长度
来源：http://chc.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://qah.sxryk.cn

[R20] 关联数组（字典）
来源：http://dml.zhixingplan.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mdm.ybcxt.top

[R21] 字符串长度
来源：http://fcv.havefunace.top

echo "${#s}"
来源：http://fog.bjfxy.top

[R22] 截取子串
来源：http://nll.yj20258.top

echo "${s:0:5}"
来源：http://mxu.redwolf501.top

[R23] 字符串替换
来源：http://jvl.jinghuilouyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bkj.guannengcc.top

[R24] 大小写转换
来源：http://lvq.ctjpmb.com

echo "${s^^}"; echo "${s,,}"
来源：http://abd.dashuyun.cn

[R25] 去后缀 / 去前缀
来源：http://rbj.redwolf501.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mdi.yj20258.top

[R26] 命令替换
来源：http://obj.xinyue.icu

now=$(date +%F); echo "$now"
来源：http://tib.jqgfzy.top

[R27] 算术展开
来源：http://xkc.tian-w.cn

echo $((1 + 2 * 3))
来源：http://scs.dashuyun.cn

[R28] 浮点运算
来源：http://okl.wangshuangyany.cn

echo "scale=2; 10/3" | bc
来源：http://rhy.epnwcf.com

[R29] 定义函数
来源：http://scr.cashguo.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://axj.andypj.xyz

[R30] 函数返回状态码
来源：http://lyo.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://jdi.smart0.xyz

[R31] 局部变量
来源：http://dfx.jiagoushi.top

f() { local x=1; echo "$x"; }
来源：http://exq.chenjidiqi.icu

[R32] 参数个数校验
来源：http://tvg.yuanzhike.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qba.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://uxi.yueranfly.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dyf.shangyingyoupin.top

[R34] 退出时清理
来源：http://goq.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://xig.hnqzz.top

[R35] 后台执行并等待
来源：http://trf.tanke756.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pfz.fzhhl.top

[R36] 并发执行多个任务
来源：http://fcy.tarul.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://etv.dashuyun.cn

[R37] 把输出赋给变量
来源：http://tyw.iojbl.cn

files=$(ls -1)
来源：http://dun.xylfe.cn

[R38] 管道串联
来源：http://uvo.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://jdm.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://enq.fehbvm.com

cmd > out.log 2>&1
来源：http://ryq.yongpay.top

[R40] 追加写日志
来源：http://tpe.yuanzhike.top

echo "log" >> out.log
来源：http://jsi.yj20258.top

[R41] 丢弃输出
来源：http://lfi.quarkkingdee.top

cmd >/dev/null 2>&1
来源：http://zhj.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://uir.gotoacloud.top

wc -l < a.txt
来源：http://ndq.pycfn.com

[R43] 按名字查找文件
来源：http://osq.andypj.xyz

find . -name "*.log" -type f
来源：http://nrv.cashguo.top

[R44] 按修改时间查找
来源：http://tdf.yueranfly.top

find . -mtime -7 -type f
来源：http://sdr.c1oappe.top

[R45] 批量删除
来源：http://zsx.yuxming.cn

find . -name "*.tmp" -delete
来源：http://cdh.svipenyu.cn

[R46] 递归替换文件内容
来源：http://ktf.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zog.ydjk.org.cn

[R47] sed 单行替换
来源：http://nar.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://fkc.c1oappe.top

[R48] awk 取指定列
来源：http://wct.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://zso.daxiang520.top

[R49] awk 带条件
来源：http://tua.jyoumei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xjf.zhaomingkeji.xyz

[R50] awk 求和
来源：http://rgj.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hac.jianghu66.top

[R51] 排序去重取前几
来源：http://zpk.gotoacloud.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zry.xylfe.cn

[R52] 统计行数
来源：http://rav.pycfn.com

wc -l a.txt
来源：http://awd.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://dys.sjlbkw.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zoa.hongshengwenyu.top

[R54] 比较两个文件
来源：http://bxz.hnqzz.top

diff a.txt b.txt
来源：http://smh.gotoacloud.top

[R55] 压缩与解压
来源：http://ykh.gzhubu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rbl.guowangkeji.top

[R56] 远程拷贝
来源：http://gwq.hesvh.cn

scp file user@host:/path/
来源：http://uyh.yuxming.cn

[R57] 远程执行命令
来源：http://ocr.ehwqpu.com

ssh user@host 'uptime'
来源：http://fmv.tianlin.xyz

[R58] 下载文件
来源：http://nlk.guowangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vha.yangfankeji.com

[R59] 发 POST JSON
来源：http://oye.ydzc1.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nlw.gaohongyu789.top

[R60] 只看 HTTP 状态码
来源：http://jnl.jiagoushi.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vff.dashuyun.cn

[R61] 磁盘占用
来源：http://yom.mhx1999.top

df -h;  du -sh *
来源：http://pqy.hcnkem.com

[R62] 找最占空间的文件
来源：http://azr.yj202588.top

du -ah . | sort -rh | head -10
来源：http://wzw.zhixingplan.top

[R63] 内存与进程
来源：http://rhc.sweek.top

free -h;  ps aux | grep nginx
来源：http://xpt.yj20258.top

[R64] 结束进程
来源：http://nhk.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://eud.zhijiandao.cn

[R65] 查看端口占用
来源：http://yfh.guannengcc.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jtg.sufxvd.cn

[R66] 定时任务
来源：http://bht.cqqwz.cn

crontab -e;  crontab -l
来源：http://zif.jinqigufen.top

[R67] 生成随机十六进制串
来源：http://dbu.vehdjk.com

openssl rand -hex 16
来源：http://xcw.52xcode.cn

[R68] 计算文件校验值
来源：http://hxs.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://all.kuanghao11.cn

[R69] 生成随机密码
来源：http://wyr.tanke756.top

head -c 16 /dev/urandom | base64
来源：http://cyf.zhixingplan.top

[R70] 时间戳与互转
来源：http://sdx.guannengcc.top

date +%s;  date -d @1700000000
来源：http://hjj.daxiang520.top

[R71] 日期格式化
来源：http://aee.snrcjt.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ijz.sxryk.cn

[R72] 等待端口就绪
来源：http://uhc.jlsjyb.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kab.pycfn.com

[R73] 分割大日志
来源：http://ahg.gogol.net.cn

split -l 1000 big.log part_
来源：http://tzu.quarkkingdee.top

[R74] 批量重命名
来源：http://fdy.jqgufenzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ilc.wangshuangyany.cn

[R75] 导出环境变量
来源：http://uys.hongshengwenyu.top

export PATH="$HOME/bin:$PATH"
来源：http://esg.zhengqikj.top

[R76] 使用临时文件
来源：http://xfq.redwolf501.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sxl.yvedp.cn

[R77] 读取用户输入
来源：http://qvu.cdnleiting.top

read -rp "请输入: " ans
来源：http://bel.guowangkeji.top

[R78] 交互式菜单
来源：http://xrr.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://orc.jinqigufen.top

[R79] 解析命令行选项
来源：http://cbr.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vyj.dashuyun.cn

[R80] 查看脚本执行耗时
来源：http://dlh.hcnkem.com

time ./run.sh
来源：http://edk.havefunace.top

================================================================================
来源：http://ggk.jinqigfzy.top

S. C / C++ 专题
来源：http://wrl.vehdjk.com

================================================================================
来源：http://zfv.haohaochexian.top

[S01] C：Hello World
来源：http://vpr.aibaodan.cn

#include <stdio.h>
来源：http://hch.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qgi.shangyingyoupin.top

[S02] C：变量与格式化输出
来源：http://lej.316326.xyz

int a = 10; printf("%d\n", a);
来源：http://uxb.zhaomingkeji.xyz

[S03] C：读入整数
来源：http://ded.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://dds.zdbjq.cn

[S04] C：字符串复制
来源：http://wvx.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://pvr.hcnkem.com

[S05] C：字符串长度
来源：http://pzj.jianghu66.top

strlen(s)
来源：http://kml.zhengqikj.top

[S06] C：字符串比较
来源：http://uqi.316326.xyz

strcmp(a, b) == 0
来源：http://pbx.vehdjk.com

[S07] C：数组遍历求和
来源：http://rtt.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gpi.xuanzx.com

[S08] C：动态内存分配与释放
来源：http://xqr.yj202588.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jcs.chenjidiqi.icu

[S09] C：结构体定义与初始化
来源：http://yui.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cae.bjfxy.top

[S10] C：指针与解引用
来源：http://iyg.9152youxi.cn

int *p = &a;  *p = 5;
来源：http://yju.gaohongyu789.top

[S11] C：逐行读文件
来源：http://mdj.sxryk.cn

FILE *f = fopen("a.txt", "r");
来源：http://gtb.fehbvm.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://xmz.havefunace.top

fclose(f);
来源：http://jnd.gotoacloud.top

[S12] C：写文件
来源：http://zny.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://liq.9152youxi.cn

[S13] C：宏定义
来源：http://ixr.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hyp.yvedp.cn

[S14] C：枚举
来源：http://qth.cheryme.top

enum Color { RED, GREEN, BLUE };
来源：http://vhe.yuxming.cn

[S15] C：类型转换
来源：http://exk.haohaochexian.top

(double) a / b
来源：http://beu.aibaodan.cn

[S16] C：位操作置位
来源：http://zgt.jyoumei.cn

x |= (1 << 3);
来源：http://rjc.fehbvm.com

[S17] C：安全拼接字符串
来源：http://njc.xuanzx.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vxi.xinyue.icu

[S18] C：命令行参数
来源：http://rcn.kuanghao11.cn

int main(int argc, char **argv)
来源：http://oib.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://ydo.sweek.top

qsort(a, n, sizeof(int), cmp);
来源：http://tmg.daxiang520.top

[S20] C：二分查找
来源：http://qol.ctjpmb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wwu.daxiang520.top

[S21] C：字符类别判断
来源：http://nou.hysaishi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mep.daria6918.cn

[S22] C：字符串转数字
来源：http://phk.shangyingyoupin.top

atoi("42");  strtod("3.14", NULL);
来源：http://usa.xuetiantiany.cn

[S23] C：随机数
来源：http://xep.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oyk.yfazqb.com

[S24] C：获取本地时间
来源：http://lzd.zdbjq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oky.yj20258.top

[S25] C：内存拷贝
来源：http://qlr.guannengcc.top

memcpy(dst, src, n);
来源：http://oqx.vqdsnc.cn

[S26] C：内存清零
来源：http://rsm.ppjwa.cn

memset(a, 0, sizeof a);
来源：http://aog.zdqjudy.top

[S27] C：定义常量
来源：http://eis.nanxuanxn.top

const double PI = 3.14159;
来源：http://pwv.hongshengwenyu.top

[S28] C：静态变量
来源：http://ljz.jqgfzy.top

static int counter = 0;
来源：http://mhi.jianghu66.top

[S29] C：变参函数
来源：http://beu.wangdashe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tdc.meibo888.top

[S30] C：头文件保护
来源：http://jkw.xylfe.cn

#ifndef X_H
来源：http://kzc.vqdsnc.cn

#define X_H
来源：http://dok.0kj1m.cn

#endif
来源：http://acy.chenlongwang.top

[S31] C++：Hello World
来源：http://qgm.nanxuanxn.top

#include <iostream>
来源：http://fem.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://oct.tanke756.top

[S32] C++：字符串
来源：http://nuz.shangyingyoupin.top

std::string s = "hi";  s += "!";
来源：http://rpc.wangdashe.top

[S33] C++：vector 增删
来源：http://dzv.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xxu.hammf.cn

[S34] C++：遍历 vector
来源：http://squ.pycfn.com

for (auto &x : v) { std::cout << x; }
来源：http://ruc.jqgfzy.top

[S35] C++：map
来源：http://tqi.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wuh.bbcook.cn

[S36] C++：unordered_map
来源：http://kus.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ele.sweek.top

[S37] C++：set
来源：http://oda.9152youxi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://crq.c1oappe.top

[S38] C++：排序
来源：http://dxq.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://hwa.cheryme.top

[S39] C++：自定义比较器排序
来源：http://klt.wangdashe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gmf.gogol.net.cn

[S40] C++：查找元素
来源：http://yrn.ydzc1.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hlh.aibaodan.cn

[S41] C++：类与构造函数
来源：http://oak.fanxiaobao.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pml.dianchejie.cn

[S42] C++：继承与虚函数
来源：http://iwv.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://apn.zdqjudy.top

[S43] C++：智能指针
来源：http://uqt.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://ysh.shanyushiyangkeji.top

[S44] C++：引用传参
来源：http://eff.yfazqb.com

void inc(int &x) { ++x; }
来源：http://fxk.hcnkem.com

[S45] C++：lambda
来源：http://oqv.yongpay.top

auto add = [](int a, int b) { return a + b; };
来源：http://xkm.yvedp.cn

[S46] C++：函数模板
来源：http://vih.jinqigfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pel.jqgfzy.top

[S47] C++：结构化绑定遍历
来源：http://nlz.hesvh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rxy.nanxuanxn.top

[S48] C++：逐行读文件
来源：http://riw.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yps.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://ydp.zdqjudy.top

[S49] C++：写文件
来源：http://xrq.jinqigfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zfk.zhongyouzk.top

[S50] C++：格式化数字
来源：http://eiu.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jtx.yfazqb.com

[S51] C++：显式类型转换
来源：http://tkt.cheryme.top

static_cast<double>(a) / b
来源：http://zgh.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://spp.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://sko.hcnkem.com

[S53] C++：移动语义
来源：http://txg.havefunace.top

std::vector<int> w = std::move(v);
来源：http://erq.iojbl.cn

[S54] C++：异常处理
来源：http://bam.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ofo.yvedp.cn

[S55] C++：结构化绑定
来源：http://mot.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qej.tarul.cn

[S56] C++：optional
来源：http://jam.gotoacloud.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://utx.jyoumei.cn

[S57] C++：编译期常量
来源：http://usm.dianchejie.cn

constexpr int N = 10;
来源：http://sin.pengpengdd.cyou

[S58] C++：命名空间
来源：http://qhv.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://xvt.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://qhr.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qxj.havefunace.top

[S60] C++：遍历并删除元素
来源：http://vfn.ivvv.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wbw.tianlin.xyz

================================================================================
来源：http://itn.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qft.chenlongwang.top

================================================================================
来源：http://hjr.svipenyu.cn

[T01] Kotlin：Hello World
来源：http://bbb.ywan-chungtsiang.top

println("Hello")
来源：http://lbw.jianghu66.top

[T02] Kotlin：变量
来源：http://enj.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zyp.zhongyouzk.top

[T03] Kotlin：字符串模板
来源：http://keq.gzhubu.top

"值: $b"
来源：http://skv.sufxvd.cn

[T04] Kotlin：空安全
来源：http://pyc.yj20258.top

val n: String? = null;  n?.length
来源：http://mdw.jianghu66.top


<!-- 参考信息 -->