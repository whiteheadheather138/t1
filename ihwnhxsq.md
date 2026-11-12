代发 wailian999

case "$1" in
来源：http://adj.tarul.cn

start) echo "启动" ;;
来源：http://pmc.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://wny.sysykeji.top

*)     echo "未知命令" ;;
来源：http://odm.shanyushiyangtech.top

esac
来源：http://ssj.ppjwa.cn

[R12] for 遍历文件
来源：http://dxh.shzxlz.cn

for f in *.txt; do echo "$f"; done
来源：http://flm.xingfuxueyuan.xyz

[R13] for 计数循环
来源：http://lxb.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://icr.ydjk.org.cn

[R14] C 风格 for
来源：http://nia.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nlm.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://ype.yuxming.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xbd.cheryme.top

[R16] until 等待条件
来源：http://uus.feifeiyinyue.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ueh.yj202588.top

[R17] 数组定义与取值
来源：http://hxm.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://miu.zhixingplan.top

[R18] 遍历数组
来源：http://orv.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bdr.gotoacloud.top

[R19] 数组长度
来源：http://paw.sweek.top

echo "${#arr[@]}"
来源：http://wkv.dashuyun.cn

[R20] 关联数组（字典）
来源：http://krh.sweek.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fdd.nanxuanxn.top

[R21] 字符串长度
来源：http://bzi.tarul.cn

echo "${#s}"
来源：http://zri.xziqi.cn

[R22] 截取子串
来源：http://qpo.nanxinkj.top

echo "${s:0:5}"
来源：http://ony.shanyushiyangtech.top

[R23] 字符串替换
来源：http://wqa.guowangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zpt.redwolf501.top

[R24] 大小写转换
来源：http://gch.9152youxi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vwy.jqgufenzy.top

[R25] 去后缀 / 去前缀
来源：http://ayl.epnwcf.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://nke.xziqi.cn

[R26] 命令替换
来源：http://qws.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://ebd.wangdashe.top

[R27] 算术展开
来源：http://tbt.hammf.cn

echo $((1 + 2 * 3))
来源：http://hza.jqgfzy.top

[R28] 浮点运算
来源：http://fye.uphjek.com

echo "scale=2; 10/3" | bc
来源：http://xkx.zhongyouzk.top

[R29] 定义函数
来源：http://xjy.hesvh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zzt.meibo888.top

[R30] 函数返回状态码
来源：http://twq.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://odo.jiagoushi.top

[R31] 局部变量
来源：http://kil.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://zpq.zdbjq.cn

[R32] 参数个数校验
来源：http://pze.yongpay.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xvk.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://meg.cheryme.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://elh.ctjpmb.com

[R34] 退出时清理
来源：http://fde.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://drr.fzhhl.top

[R35] 后台执行并等待
来源：http://kar.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jxm.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://skl.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zsd.redwolf501.top

[R37] 把输出赋给变量
来源：http://fpw.chenjidiqi.icu

files=$(ls -1)
来源：http://pka.snrcjt.cn

[R38] 管道串联
来源：http://xrp.yongpay.top

cat a.txt | grep -i error | wc -l
来源：http://yat.jinghuilouyu.cn

[R39] 重定向标准输出与错误
来源：http://izl.xuanzx.com

cmd > out.log 2>&1
来源：http://etr.aizwys.cn

[R40] 追加写日志
来源：http://bfi.feifeiyinyue.top

echo "log" >> out.log
来源：http://nkk.smart0.xyz

[R41] 丢弃输出
来源：http://bwj.hysaishi.cn

cmd >/dev/null 2>&1
来源：http://gyc.shzxlz.cn

[R42] 输入重定向
来源：http://xur.xziqi.cn

wc -l < a.txt
来源：http://itf.yj202588.top

[R43] 按名字查找文件
来源：http://cph.yuxming.cn

find . -name "*.log" -type f
来源：http://wbl.jqgfzy.top

[R44] 按修改时间查找
来源：http://ahm.ywan-chungtsiang.top

find . -mtime -7 -type f
来源：http://mfm.ctjpmb.com

[R45] 批量删除
来源：http://gvo.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://tlg.yvedp.cn

[R46] 递归替换文件内容
来源：http://mku.yuanzhike.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gzc.hywenlv.cn

[R47] sed 单行替换
来源：http://mps.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://jsv.tarul.cn

[R48] awk 取指定列
来源：http://elw.uphjek.com

awk '{print $1, $3}' a.txt
来源：http://wqe.ctjpmb.com

[R49] awk 带条件
来源：http://rge.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xih.pengpengdd.cyou

[R50] awk 求和
来源：http://lse.zhijiandao.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ick.hesvh.cn

[R51] 排序去重取前几
来源：http://hhm.yuanzhike.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wti.gzhubu.top

[R52] 统计行数
来源：http://ior.zdbjq.cn

wc -l a.txt
来源：http://tkb.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://lle.vehdjk.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zup.yongpay.top

[R54] 比较两个文件
来源：http://ulx.c1oappe.top

diff a.txt b.txt
来源：http://zcn.hnqzz.top

[R55] 压缩与解压
来源：http://uvk.daria6918.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ugz.hesvh.cn

[R56] 远程拷贝
来源：http://waa.vqdsnc.cn

scp file user@host:/path/
来源：http://kgp.jqgfzy.top

[R57] 远程执行命令
来源：http://xzg.aibaodan.cn

ssh user@host 'uptime'
来源：http://nev.vqdsnc.cn

[R58] 下载文件
来源：http://gec.jianghu66.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wxv.gogol.net.cn

[R59] 发 POST JSON
来源：http://uqx.sysykeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bvi.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://ixj.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lrh.hysaishi.cn

[R61] 磁盘占用
来源：http://pqb.zhijiandao.cn

df -h;  du -sh *
来源：http://dbp.cucudq.cn

[R62] 找最占空间的文件
来源：http://brk.cashguo.top

du -ah . | sort -rh | head -10
来源：http://rln.nwbrower.top

[R63] 内存与进程
来源：http://yzc.yonumen.top

free -h;  ps aux | grep nginx
来源：http://vmm.hesvh.cn

[R64] 结束进程
来源：http://ldf.fktsv.cn

kill -9 $(pgrep -f app.py)
来源：http://udx.zhiwuduotai.top

[R65] 查看端口占用
来源：http://cib.jqgfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zss.jinqigfzy.top

[R66] 定时任务
来源：http://qvq.jinqigufen.top

crontab -e;  crontab -l
来源：http://qxw.pengpengdd.cyou

[R67] 生成随机十六进制串
来源：http://wac.jqgfzy.top

openssl rand -hex 16
来源：http://opf.xuanzx.com

[R68] 计算文件校验值
来源：http://elh.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vzd.yuxming.cn

[R69] 生成随机密码
来源：http://als.yj20258.top

head -c 16 /dev/urandom | base64
来源：http://lxb.birdmap.top

[R70] 时间戳与互转
来源：http://qcv.cqqwz.cn

date +%s;  date -d @1700000000
来源：http://shm.zhijiandao.cn

[R71] 日期格式化
来源：http://uwj.wangdashe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xvw.pengpengdd.cyou

[R72] 等待端口就绪
来源：http://wuh.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yaf.hnxiangtu.top

[R73] 分割大日志
来源：http://qwl.wangshuangyany.cn

split -l 1000 big.log part_
来源：http://rsq.zhiwuduotai.top

[R74] 批量重命名
来源：http://irq.zycfv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://asv.hysaishi.cn

[R75] 导出环境变量
来源：http://vte.ppjwa.cn

export PATH="$HOME/bin:$PATH"
来源：http://udk.gzhubu.top

[R76] 使用临时文件
来源：http://bfp.yanxiufei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fku.cheryme.top

[R77] 读取用户输入
来源：http://umj.xuetiantiany.cn

read -rp "请输入: " ans
来源：http://yqw.uphjek.com

[R78] 交互式菜单
来源：http://mtq.bbcook.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oia.tian-w.cn

[R79] 解析命令行选项
来源：http://yao.hammf.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ytn.iojbl.cn

[R80] 查看脚本执行耗时
来源：http://nky.hfpthk.cn

time ./run.sh
来源：http://dok.dianchejie.cn

================================================================================
来源：http://xbm.ctjpmb.com

S. C / C++ 专题
来源：http://pxa.316326.xyz

================================================================================
来源：http://pqb.ehwqpu.com

[S01] C：Hello World
来源：http://uxs.jianghu66.top

#include <stdio.h>
来源：http://pps.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qug.jinyuanbaomall.cn

[S02] C：变量与格式化输出
来源：http://nfq.zdbjq.cn

int a = 10; printf("%d\n", a);
来源：http://rec.zhijiandao.cn

[S03] C：读入整数
来源：http://zim.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://irx.sweek.top

[S04] C：字符串复制
来源：http://rnm.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://yzx.yj20258.top

[S05] C：字符串长度
来源：http://inp.fzhhl.top

strlen(s)
来源：http://kqz.jqgufenzy.top

[S06] C：字符串比较
来源：http://smm.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://pjl.meibo888.top

[S07] C：数组遍历求和
来源：http://dxd.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bjl.52xcode.cn

[S08] C：动态内存分配与释放
来源：http://him.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ufk.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://ssz.birdmap.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://msw.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://faf.jlsjyb.cn

int *p = &a;  *p = 5;
来源：http://wth.jyoumei.cn

[S11] C：逐行读文件
来源：http://iyd.yj202588.top

FILE *f = fopen("a.txt", "r");
来源：http://whe.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://giw.zhengqikj.top

fclose(f);
来源：http://wit.daria6918.cn

[S12] C：写文件
来源：http://rjh.dashuyun.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bkr.ivvv.top

[S13] C：宏定义
来源：http://caf.daxiang520.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wcv.hnqzz.top

[S14] C：枚举
来源：http://rjz.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://zfn.yj202588.top

[S15] C：类型转换
来源：http://tfl.gogol.net.cn

(double) a / b
来源：http://dfv.hywenlv.cn

[S16] C：位操作置位
来源：http://wvv.tian-w.cn

x |= (1 << 3);
来源：http://pah.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://oin.yvedp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zeh.hammf.cn

[S18] C：命令行参数
来源：http://anb.hysaishi.cn

int main(int argc, char **argv)
来源：http://iry.meibo888.top

[S19] C：快速排序
来源：http://dvd.jiagoushi.top

qsort(a, n, sizeof(int), cmp);
来源：http://tpn.fehbvm.com

[S20] C：二分查找
来源：http://pwr.wangshuangyany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nud.cashguo.top

[S21] C：字符类别判断
来源：http://byf.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kfr.tanke756.top

[S22] C：字符串转数字
来源：http://ncx.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://bsp.0kj1m.cn

[S23] C：随机数
来源：http://tps.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fqh.pengpengdd.cyou

[S24] C：获取本地时间
来源：http://eub.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://edn.xziqi.cn

[S25] C：内存拷贝
来源：http://tod.zhiwuduotai.top

memcpy(dst, src, n);
来源：http://jfu.zdbjq.cn

[S26] C：内存清零
来源：http://qnl.iojbl.cn

memset(a, 0, sizeof a);
来源：http://vom.bjfxy.top

[S27] C：定义常量
来源：http://woe.meibo888.top

const double PI = 3.14159;
来源：http://skp.zycfv.cn

[S28] C：静态变量
来源：http://wwf.sjlbkw.cn

static int counter = 0;
来源：http://hfc.nanxinkj.top

[S29] C：变参函数
来源：http://zdm.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yxw.fzhhl.top

[S30] C：头文件保护
来源：http://nka.52xcode.cn

#ifndef X_H
来源：http://yel.birdmap.top

#define X_H
来源：http://fdw.yangfankeji.com

#endif
来源：http://sxn.zdqjudy.top

[S31] C++：Hello World
来源：http://vqj.nanxinkj.top

#include <iostream>
来源：http://sjf.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://esf.cqqwz.cn

[S32] C++：字符串
来源：http://vif.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://erg.316326.xyz

[S33] C++：vector 增删
来源：http://cnv.andypj.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lal.xylfe.cn

[S34] C++：遍历 vector
来源：http://oic.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://amb.smart0.xyz

[S35] C++：map
来源：http://cgf.jinghuilouyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mqq.andypj.xyz

[S36] C++：unordered_map
来源：http://xjx.sufxvd.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jtn.haohaochexian.top

[S37] C++：set
来源：http://nkm.chenjidiqi.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kxc.shanyushiyangkeji.top

[S38] C++：排序
来源：http://qmb.svipenyu.cn

std::sort(v.begin(), v.end());
来源：http://hsz.zdqjudy.top

[S39] C++：自定义比较器排序
来源：http://fjt.fktsv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qde.cheryme.top

[S40] C++：查找元素
来源：http://did.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kne.cheryme.top

[S41] C++：类与构造函数
来源：http://oys.daxiang520.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://muv.jqgufenzy.top

[S42] C++：继承与虚函数
来源：http://gqq.zhoulong.xyz

class B : public Base { public: void f() override {} };
来源：http://dmb.gotoacloud.top

[S43] C++：智能指针
来源：http://eku.hnqzz.top

auto p = std::make_unique<int>(5);
来源：http://qgd.tarul.cn

[S44] C++：引用传参
来源：http://mdn.yj20258.top

void inc(int &x) { ++x; }
来源：http://bwc.zhoulong.xyz

[S45] C++：lambda
来源：http://kti.epnwcf.com

auto add = [](int a, int b) { return a + b; };
来源：http://knu.mhx1999.top

[S46] C++：函数模板
来源：http://xhf.yfazqb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pvt.nanxuanxn.top

[S47] C++：结构化绑定遍历
来源：http://ywn.gaohongyu789.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sud.yuxming.cn

[S48] C++：逐行读文件
来源：http://bbi.316326.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://ovr.fktsv.cn

while (std::getline(in, line)) { }
来源：http://mxu.tanke756.top

[S49] C++：写文件
来源：http://pmb.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hbl.gotoacloud.top

[S50] C++：格式化数字
来源：http://nqw.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rlb.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://mhr.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://yro.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://zip.gzhubu.top

int size() const noexcept { return n_; }
来源：http://btc.cheryme.top

[S53] C++：移动语义
来源：http://cvx.dianchejie.cn

std::vector<int> w = std::move(v);
来源：http://uvo.zhixingplan.top

[S54] C++：异常处理
来源：http://rmn.chenlongwang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rvi.wangdashe.top

[S55] C++：结构化绑定
来源：http://phd.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://lzy.xuetiantiany.cn

[S56] C++：optional
来源：http://vxg.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tsh.smart0.xyz

[S57] C++：编译期常量
来源：http://wla.yongpay.top

constexpr int N = 10;
来源：http://mup.cashguo.top

[S58] C++：命名空间
来源：http://pfo.daxiang520.top

namespace ns { int f() { return 1; } }
来源：http://ubs.kuanghao11.cn

[S59] C++：静态断言
来源：http://sqe.zhixingplan.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sse.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://bgr.haohaochexian.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zhx.svipenyu.cn

================================================================================
来源：http://fgk.hongshengwenyu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sqr.fanxiaobao.xyz

================================================================================
来源：http://ygq.fengsongda.top

[T01] Kotlin：Hello World
来源：http://faq.jinqigfzy.top

println("Hello")
来源：http://bnd.dianchejie.cn

[T02] Kotlin：变量
来源：http://rmd.sxryk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://boi.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://jtk.mhx1999.top

"值: $b"
来源：http://chg.chenlongwang.top

[T04] Kotlin：空安全
来源：http://oad.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://iqu.cheryme.top

[T05] Kotlin：when 表达式
来源：http://mou.wangdashe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uvl.guannengcc.top

[T06] Kotlin：集合映射
来源：http://dnf.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://urs.xinyue.icu

[T07] Kotlin：集合过滤
来源：http://nea.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jzk.ybcxt.top

[T08] Kotlin：数据类
来源：http://ckg.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://bsk.zhoulong.xyz

[T09] Kotlin：扩展函数
来源：http://saa.nanxuanxn.top

fun String.exclaim() = this + "!"
来源：http://kux.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://lee.dashuyun.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ovj.xinyue.icu

[T11] Kotlin：协程
来源：http://evk.ydjk.org.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zze.yangfankeji.com

[T12] Kotlin：解构声明
来源：http://mbh.jinghuilouyu.cn

val (a, b) = Pair(1, 2)
来源：http://hiw.gogol.net.cn


<!-- 参考信息 -->