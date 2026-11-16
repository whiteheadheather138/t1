代发 wailian999

case "$1" in
来源：http://ozk.tianlin.xyz

start) echo "启动" ;;
来源：http://fwj.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://hjq.fehbvm.com

*)     echo "未知命令" ;;
来源：http://uiz.zhiwuduotai.top

esac
来源：http://zmg.mhx1999.top

[R12] for 遍历文件
来源：http://fwl.ivvv.top

for f in *.txt; do echo "$f"; done
来源：http://kdc.xuetiantiany.cn

[R13] for 计数循环
来源：http://vdg.jqgfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://kej.0kj1m.cn

[R14] C 风格 for
来源：http://tsz.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oft.0kj1m.cn

[R15] while 逐行读文件
来源：http://dvu.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vdl.yonumen.top

[R16] until 等待条件
来源：http://qxj.yj20258888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ryh.sjlbkw.cn

[R17] 数组定义与取值
来源：http://vcl.hongshengwenyu.top

arr=(a b c); echo "${arr[0]}"
来源：http://ayd.yfazqb.com

[R18] 遍历数组
来源：http://lml.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aln.cashguo.top

[R19] 数组长度
来源：http://mkx.cqqwz.cn

echo "${#arr[@]}"
来源：http://fcm.hywenlv.cn

[R20] 关联数组（字典）
来源：http://bcg.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cmi.xuetiantiany.cn

[R21] 字符串长度
来源：http://ncx.sufxvd.cn

echo "${#s}"
来源：http://bic.sxryk.cn

[R22] 截取子串
来源：http://dik.bjfxy.top

echo "${s:0:5}"
来源：http://dml.c1oappe.top

[R23] 字符串替换
来源：http://jxs.zhoulong.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jhd.zhixingplan.top

[R24] 大小写转换
来源：http://ina.ivvv.top

echo "${s^^}"; echo "${s,,}"
来源：http://vdj.wangshuangyany.cn

[R25] 去后缀 / 去前缀
来源：http://ngw.yfazqb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://bca.pengpengdd.cyou

[R26] 命令替换
来源：http://mdg.0kj1m.cn

now=$(date +%F); echo "$now"
来源：http://dpp.feifeiyinyue.top

[R27] 算术展开
来源：http://uvw.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://hjl.ydzc1.top

[R28] 浮点运算
来源：http://mky.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://dfp.smart0.xyz

[R29] 定义函数
来源：http://tyu.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://umk.wangshuangyany.cn

[R30] 函数返回状态码
来源：http://cuj.jianghu66.top

f() { return 0; }; f || echo "失败了"
来源：http://dfp.uphjek.com

[R31] 局部变量
来源：http://fbm.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://zrp.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://bzg.cashguo.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dgl.tarul.cn

[R33] 捕获错误并提示行号
来源：http://tfh.sweek.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rdw.chenzaomai.com

[R34] 退出时清理
来源：http://vtd.jqgufenzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://iou.pycfn.com

[R35] 后台执行并等待
来源：http://yuj.0kj1m.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kvq.zdqjudy.top

[R36] 并发执行多个任务
来源：http://ngs.fzhhl.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tyv.gaohongyu789.top

[R37] 把输出赋给变量
来源：http://plc.tarul.cn

files=$(ls -1)
来源：http://pgz.gaohongyu789.top

[R38] 管道串联
来源：http://bgd.kuanghao11.cn

cat a.txt | grep -i error | wc -l
来源：http://hit.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://ico.0kj1m.cn

cmd > out.log 2>&1
来源：http://jqj.nanxuanxn.top

[R40] 追加写日志
来源：http://ahm.zhixingplan.top

echo "log" >> out.log
来源：http://oje.yangfankeji.com

[R41] 丢弃输出
来源：http://nft.yj202588.top

cmd >/dev/null 2>&1
来源：http://jsn.yuxming.cn

[R42] 输入重定向
来源：http://wjm.bbcook.cn

wc -l < a.txt
来源：http://wbb.fzhhl.top

[R43] 按名字查找文件
来源：http://hrc.ydzc1.top

find . -name "*.log" -type f
来源：http://ghy.guannengcc.top

[R44] 按修改时间查找
来源：http://dua.zdqjudy.top

find . -mtime -7 -type f
来源：http://zno.sweek.top

[R45] 批量删除
来源：http://ied.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://xzg.hammf.cn

[R46] 递归替换文件内容
来源：http://ezx.jinyuanbaomall.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qps.hesvh.cn

[R47] sed 单行替换
来源：http://fyc.yfazqb.com

sed -i 's/foo/bar/g' a.txt
来源：http://afx.cucudq.cn

[R48] awk 取指定列
来源：http://khr.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://nlz.haohaochexian.top

[R49] awk 带条件
来源：http://dpn.gogol.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mgq.yuanzhike.top

[R50] awk 求和
来源：http://jfj.shanyushiyangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://wqd.wangdashe.top

[R51] 排序去重取前几
来源：http://ela.316326.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://cnx.zdqjudy.top

[R52] 统计行数
来源：http://sbe.sufxvd.cn

wc -l a.txt
来源：http://iwt.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://euo.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jas.aizwys.cn

[R54] 比较两个文件
来源：http://aqz.aizwys.cn

diff a.txt b.txt
来源：http://vkh.birdmap.top

[R55] 压缩与解压
来源：http://wwj.zhixingplan.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ngw.sxryk.cn

[R56] 远程拷贝
来源：http://gco.tian-w.cn

scp file user@host:/path/
来源：http://qtw.jinqigfzy.top

[R57] 远程执行命令
来源：http://hjn.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://jvm.ybcxt.top

[R58] 下载文件
来源：http://sdi.chenjidiqi.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mwe.nanxuanxn.top

[R59] 发 POST JSON
来源：http://qva.hcnkem.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vbk.yj20258888.top

[R60] 只看 HTTP 状态码
来源：http://djj.ydzc1.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tis.yonumen.top

[R61] 磁盘占用
来源：http://rne.birdmap.top

df -h;  du -sh *
来源：http://mwc.zhaomingkeji.xyz

[R62] 找最占空间的文件
来源：http://yud.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://dwb.sxryk.cn

[R63] 内存与进程
来源：http://twc.bbcook.cn

free -h;  ps aux | grep nginx
来源：http://fmy.vqdsnc.cn

[R64] 结束进程
来源：http://ubo.jqgfzy.top

kill -9 $(pgrep -f app.py)
来源：http://gvy.shuidangran.top

[R65] 查看端口占用
来源：http://dpn.kuanghao11.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gxj.fehbvm.com

[R66] 定时任务
来源：http://rpm.jinghuilouyu.cn

crontab -e;  crontab -l
来源：http://oqc.sysykeji.top

[R67] 生成随机十六进制串
来源：http://ngx.redwolf501.top

openssl rand -hex 16
来源：http://sqe.aizwys.cn

[R68] 计算文件校验值
来源：http://yrf.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://lon.fengsongda.top

[R69] 生成随机密码
来源：http://dbm.sjlbkw.cn

head -c 16 /dev/urandom | base64
来源：http://mhu.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://rws.cucudq.cn

date +%s;  date -d @1700000000
来源：http://avx.xziqi.cn

[R71] 日期格式化
来源：http://ovd.kuanghao11.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://biu.xylfe.cn

[R72] 等待端口就绪
来源：http://ass.gotoacloud.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rdp.xuetiantiany.cn

[R73] 分割大日志
来源：http://wit.gotoacloud.top

split -l 1000 big.log part_
来源：http://ekc.chenlongwang.top

[R74] 批量重命名
来源：http://epd.zhoulong.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ovj.chenzaomai.com

[R75] 导出环境变量
来源：http://erl.sxryk.cn

export PATH="$HOME/bin:$PATH"
来源：http://txf.vehdjk.com

[R76] 使用临时文件
来源：http://nri.nanxinkj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xmu.aibaodan.cn

[R77] 读取用户输入
来源：http://hnt.yongpay.top

read -rp "请输入: " ans
来源：http://stq.tanke756.top

[R78] 交互式菜单
来源：http://clk.shzxlz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fov.chenzaomai.com

[R79] 解析命令行选项
来源：http://lrb.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mio.yvedp.cn

[R80] 查看脚本执行耗时
来源：http://sfy.zhaomingkeji.xyz

time ./run.sh
来源：http://xsn.yfazqb.com

================================================================================
来源：http://zhq.hammf.cn

S. C / C++ 专题
来源：http://kkf.jinghuilouyu.cn

================================================================================
来源：http://ukm.shanyushiyangtech.top

[S01] C：Hello World
来源：http://hzr.epnwcf.com

#include <stdio.h>
来源：http://iex.wangshuangyany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wja.jiagoushi.top

[S02] C：变量与格式化输出
来源：http://pho.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://jwb.zdbjq.cn

[S03] C：读入整数
来源：http://ysx.zhoulong.xyz

int x; scanf("%d", &x);
来源：http://xhh.havefunace.top

[S04] C：字符串复制
来源：http://mzq.zhongyouzk.top

char dst[32]; strcpy(dst, "hi");
来源：http://ynh.sufxvd.cn

[S05] C：字符串长度
来源：http://ruv.pengpengdd.cyou

strlen(s)
来源：http://pzt.nanxuanxn.top

[S06] C：字符串比较
来源：http://hud.jinghuilouyu.cn

strcmp(a, b) == 0
来源：http://ofe.smart0.xyz

[S07] C：数组遍历求和
来源：http://csz.xziqi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vgy.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://hlu.0kj1m.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://udl.xinyue.icu

[S09] C：结构体定义与初始化
来源：http://frt.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lve.smart0.xyz

[S10] C：指针与解引用
来源：http://tsg.yuxming.cn

int *p = &a;  *p = 5;
来源：http://cho.smart0.xyz

[S11] C：逐行读文件
来源：http://ist.daria6918.cn

FILE *f = fopen("a.txt", "r");
来源：http://plx.shuidangran.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ufh.kuanghao11.cn

fclose(f);
来源：http://qhe.xinyue.icu

[S12] C：写文件
来源：http://jmq.316326.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://myx.yuanzhike.top

[S13] C：宏定义
来源：http://qgp.gogol.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hzn.ydzc1.top

[S14] C：枚举
来源：http://ofm.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://zbu.vehdjk.com

[S15] C：类型转换
来源：http://sea.xingfuxueyuan.xyz

(double) a / b
来源：http://dms.cashguo.top

[S16] C：位操作置位
来源：http://mtb.guannengcc.top

x |= (1 << 3);
来源：http://thz.hesvh.cn

[S17] C：安全拼接字符串
来源：http://okl.hongshengwenyu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kci.redwolf501.top

[S18] C：命令行参数
来源：http://peo.jlsjyb.cn

int main(int argc, char **argv)
来源：http://bzb.redwolf501.top

[S19] C：快速排序
来源：http://ohg.tanke756.top

qsort(a, n, sizeof(int), cmp);
来源：http://shx.jinqigufen.top

[S20] C：二分查找
来源：http://uft.shuidangran.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cne.pycfn.com

[S21] C：字符类别判断
来源：http://ksm.hesvh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://trg.yvedp.cn

[S22] C：字符串转数字
来源：http://vqy.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://hpb.sweek.top

[S23] C：随机数
来源：http://wfm.jinyuanbaomall.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gok.gzhubu.top

[S24] C：获取本地时间
来源：http://fia.yueranfly.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rin.hammf.cn

[S25] C：内存拷贝
来源：http://mwr.hesvh.cn

memcpy(dst, src, n);
来源：http://zwr.tarul.cn

[S26] C：内存清零
来源：http://lgf.ivvv.top

memset(a, 0, sizeof a);
来源：http://nls.nanxuanxn.top

[S27] C：定义常量
来源：http://rbn.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://qvo.sweek.top

[S28] C：静态变量
来源：http://czy.shzxlz.cn

static int counter = 0;
来源：http://rdv.xinyue.icu

[S29] C：变参函数
来源：http://hfl.yfazqb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ztp.yj20258888.top

[S30] C：头文件保护
来源：http://ofa.zhaomingkeji.xyz

#ifndef X_H
来源：http://opf.jinghuilouyu.cn

#define X_H
来源：http://rsi.birdmap.top

#endif
来源：http://qnj.jinqigfzy.top

[S31] C++：Hello World
来源：http://pjg.hammf.cn

#include <iostream>
来源：http://lvt.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://zkv.yuanzhike.top

[S32] C++：字符串
来源：http://sbg.316326.xyz

std::string s = "hi";  s += "!";
来源：http://bdt.xingfuxueyuan.xyz

[S33] C++：vector 增删
来源：http://lgb.tanke756.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bkc.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://ncw.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://dfu.nanxinkj.top

[S35] C++：map
来源：http://cov.hysaishi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vfa.yj202588.top

[S36] C++：unordered_map
来源：http://prm.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://div.snrcjt.cn

[S37] C++：set
来源：http://csl.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cvk.gaohongyu789.top

[S38] C++：排序
来源：http://pin.zhengqikj.top

std::sort(v.begin(), v.end());
来源：http://oab.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://fte.haohaochexian.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pea.hesvh.cn

[S40] C++：查找元素
来源：http://vre.nwbrower.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rog.ehwqpu.com

[S41] C++：类与构造函数
来源：http://ezu.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xwz.fzhhl.top

[S42] C++：继承与虚函数
来源：http://byv.pengpengdd.cyou

class B : public Base { public: void f() override {} };
来源：http://oqj.zhengqikj.top

[S43] C++：智能指针
来源：http://foy.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://lww.ydjk.org.cn

[S44] C++：引用传参
来源：http://lvl.316326.xyz

void inc(int &x) { ++x; }
来源：http://vxs.yfazqb.com

[S45] C++：lambda
来源：http://afa.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://pfj.jlsjyb.cn

[S46] C++：函数模板
来源：http://cjj.quarkkingdee.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://opl.dashuyun.cn

[S47] C++：结构化绑定遍历
来源：http://beo.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bqv.svipenyu.cn

[S48] C++：逐行读文件
来源：http://bbh.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://pqi.jinghuilouyu.cn

while (std::getline(in, line)) { }
来源：http://rhg.yj20258888.top

[S49] C++：写文件
来源：http://wbr.zdbjq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rmz.cashguo.top

[S50] C++：格式化数字
来源：http://jly.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tum.ivvv.top

[S51] C++：显式类型转换
来源：http://epc.jiagoushi.top

static_cast<double>(a) / b
来源：http://cmc.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://eac.vehdjk.com

int size() const noexcept { return n_; }
来源：http://lhb.gzhubu.top

[S53] C++：移动语义
来源：http://riy.gzhubu.top

std::vector<int> w = std::move(v);
来源：http://tta.yvedp.cn

[S54] C++：异常处理
来源：http://qum.chenlongwang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uqi.zdbjq.cn

[S55] C++：结构化绑定
来源：http://ffw.9152youxi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bni.yonumen.top

[S56] C++：optional
来源：http://tph.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dkk.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://xep.shuidangran.top

constexpr int N = 10;
来源：http://osc.nanxuanxn.top

[S58] C++：命名空间
来源：http://lyq.zdqjudy.top

namespace ns { int f() { return 1; } }
来源：http://fdr.zhijiandao.cn

[S59] C++：静态断言
来源：http://qom.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://raz.ppjwa.cn

[S60] C++：遍历并删除元素
来源：http://jzz.ppjwa.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jxn.birdmap.top

================================================================================
来源：http://trw.andypj.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iuh.gaohongyu789.top

================================================================================
来源：http://hlp.xziqi.cn

[T01] Kotlin：Hello World
来源：http://glz.hcnkem.com

println("Hello")
来源：http://snw.aizwys.cn

[T02] Kotlin：变量
来源：http://wfi.jqgufenzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ehx.jqgfzy.top

[T03] Kotlin：字符串模板
来源：http://two.zdqjudy.top

"值: $b"
来源：http://ykk.yueranfly.top

[T04] Kotlin：空安全
来源：http://gun.zdbjq.cn

val n: String? = null;  n?.length
来源：http://ppl.fengsongda.top

[T05] Kotlin：when 表达式
来源：http://orv.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qdp.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://qvi.wangdashe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zhj.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://cox.cucudq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hav.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://wrj.ydjk.org.cn

data class User(val name: String, val age: Int)
来源：http://zcj.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://gpk.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://pnv.svipenyu.cn

[T10] Kotlin：默认参数
来源：http://mvy.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://avd.hongshengwenyu.top

[T11] Kotlin：协程
来源：http://ftv.fehbvm.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://vlk.hnxiangtu.top

[T12] Kotlin：解构声明
来源：http://xvs.dianchejie.cn

val (a, b) = Pair(1, 2)
来源：http://nil.fktsv.cn


<!-- 参考信息 -->