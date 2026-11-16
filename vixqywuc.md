代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://asm.nwbrower.top

[R10] 正则匹配
来源：http://moh.zhoulong.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iaq.52xcode.cn

[R11] case 多分支
来源：http://umd.c1oappe.top

case "$1" in
来源：http://znq.cdnleiting.top

start) echo "启动" ;;
来源：http://ltf.fktsv.cn

stop)  echo "停止" ;;
来源：http://gjb.yanxiufei.cn

*)     echo "未知命令" ;;
来源：http://pvs.aibaodan.cn

esac
来源：http://evj.meibo888.top

[R12] for 遍历文件
来源：http://bjm.fzhhl.top

for f in *.txt; do echo "$f"; done
来源：http://amg.jinyuanbaomall.cn

[R13] for 计数循环
来源：http://hqa.zhixingplan.top

for i in {1..10}; do echo "$i"; done
来源：http://tyv.zycfv.cn

[R14] C 风格 for
来源：http://pfj.hnxiangtu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ugk.xinyue.icu

[R15] while 逐行读文件
来源：http://cyf.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kgm.dashuyun.cn

[R16] until 等待条件
来源：http://gre.hnqzz.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xqk.aizwys.cn

[R17] 数组定义与取值
来源：http://aib.fktsv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jzn.jinyuanbaomall.cn

[R18] 遍历数组
来源：http://jtw.yj20258.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ujm.aibaodan.cn

[R19] 数组长度
来源：http://unf.jianghu66.top

echo "${#arr[@]}"
来源：http://udz.yuxming.cn

[R20] 关联数组（字典）
来源：http://phw.xinyue.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://akx.9152youxi.cn

[R21] 字符串长度
来源：http://axx.zhengqikj.top

echo "${#s}"
来源：http://zgr.xinyue.icu

[R22] 截取子串
来源：http://ivt.fzhhl.top

echo "${s:0:5}"
来源：http://aga.yanxiufei.cn

[R23] 字符串替换
来源：http://hcg.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sfg.wangshuangyany.cn

[R24] 大小写转换
来源：http://esv.shzxlz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ahw.jinyuanbaomall.cn

[R25] 去后缀 / 去前缀
来源：http://qyn.jianghu66.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jxx.bjfxy.top

[R26] 命令替换
来源：http://miz.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://aht.zycfv.cn

[R27] 算术展开
来源：http://nyv.daria6918.cn

echo $((1 + 2 * 3))
来源：http://ido.jinghuilouyu.cn

[R28] 浮点运算
来源：http://hod.iojbl.cn

echo "scale=2; 10/3" | bc
来源：http://ela.yanxiufei.cn

[R29] 定义函数
来源：http://nuk.vehdjk.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aox.quarkkingdee.top

[R30] 函数返回状态码
来源：http://cet.yanxiufei.cn

f() { return 0; }; f || echo "失败了"
来源：http://sao.xuanzx.com

[R31] 局部变量
来源：http://qsl.xingfuxueyuan.xyz

f() { local x=1; echo "$x"; }
来源：http://wmn.xziqi.cn

[R32] 参数个数校验
来源：http://zqw.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mzv.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://kwm.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://shk.nanxinkj.top

[R34] 退出时清理
来源：http://bsd.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://owm.shzxlz.cn

[R35] 后台执行并等待
来源：http://ipf.ehwqpu.com

sleep 5 & pid=$!; wait "$pid"
来源：http://chq.haohaochexian.top

[R36] 并发执行多个任务
来源：http://gyz.svipenyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jgf.pycfn.com

[R37] 把输出赋给变量
来源：http://jmx.tianlin.xyz

files=$(ls -1)
来源：http://nuh.havefunace.top

[R38] 管道串联
来源：http://gdt.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://txw.bbcook.cn

[R39] 重定向标准输出与错误
来源：http://bpv.sysykeji.top

cmd > out.log 2>&1
来源：http://eor.mhx1999.top

[R40] 追加写日志
来源：http://nss.316326.xyz

echo "log" >> out.log
来源：http://chg.snrcjt.cn

[R41] 丢弃输出
来源：http://chh.fktsv.cn

cmd >/dev/null 2>&1
来源：http://tsg.svipenyu.cn

[R42] 输入重定向
来源：http://vpy.bbcook.cn

wc -l < a.txt
来源：http://uyj.mhx1999.top

[R43] 按名字查找文件
来源：http://mbq.svipenyu.cn

find . -name "*.log" -type f
来源：http://uhq.jiagoushi.top

[R44] 按修改时间查找
来源：http://jkj.nwbrower.top

find . -mtime -7 -type f
来源：http://qzy.jiagoushi.top

[R45] 批量删除
来源：http://kls.iojbl.cn

find . -name "*.tmp" -delete
来源：http://vit.epnwcf.com

[R46] 递归替换文件内容
来源：http://sic.hysaishi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bfn.feifeiyinyue.top

[R47] sed 单行替换
来源：http://ayi.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://hbi.birdmap.top

[R48] awk 取指定列
来源：http://liv.uphjek.com

awk '{print $1, $3}' a.txt
来源：http://ibv.jqgfzy.top

[R49] awk 带条件
来源：http://rtc.gaohongyu789.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cgm.tian-w.cn

[R50] awk 求和
来源：http://rbs.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tno.ydjk.org.cn

[R51] 排序去重取前几
来源：http://cxs.dianchejie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://aqn.tian-w.cn

[R52] 统计行数
来源：http://yys.yueranfly.top

wc -l a.txt
来源：http://bfc.pengpengdd.cyou

[R53] 查看文件头与实时尾
来源：http://ibk.bjfxy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xtp.gaohongyu789.top

[R54] 比较两个文件
来源：http://uny.xuetiantiany.cn

diff a.txt b.txt
来源：http://zcj.yfazqb.com

[R55] 压缩与解压
来源：http://nyp.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ese.nanxinkj.top

[R56] 远程拷贝
来源：http://urt.xuanzx.com

scp file user@host:/path/
来源：http://bos.meibo888.top

[R57] 远程执行命令
来源：http://ahq.yangfankeji.com

ssh user@host 'uptime'
来源：http://ckg.cqqwz.cn

[R58] 下载文件
来源：http://bzv.9152youxi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://auu.hysaishi.cn

[R59] 发 POST JSON
来源：http://dsh.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nrl.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://bom.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xck.ivvv.top

[R61] 磁盘占用
来源：http://baw.yj202588.top

df -h;  du -sh *
来源：http://hqg.zdqjudy.top

[R62] 找最占空间的文件
来源：http://uzk.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://ycw.ctjpmb.com

[R63] 内存与进程
来源：http://usy.zdbjq.cn

free -h;  ps aux | grep nginx
来源：http://iuu.jinqigufen.top

[R64] 结束进程
来源：http://zsu.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://xtc.cqqwz.cn

[R65] 查看端口占用
来源：http://vdu.meibo888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oky.sysykeji.top

[R66] 定时任务
来源：http://idp.hcnkem.com

crontab -e;  crontab -l
来源：http://trs.316326.xyz

[R67] 生成随机十六进制串
来源：http://xla.kuanghao11.cn

openssl rand -hex 16
来源：http://usa.yueranfly.top

[R68] 计算文件校验值
来源：http://ayz.daria6918.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ktq.jinyuanbaomall.cn

[R69] 生成随机密码
来源：http://axs.andypj.xyz

head -c 16 /dev/urandom | base64
来源：http://uim.sweek.top

[R70] 时间戳与互转
来源：http://jqe.yangfankeji.com

date +%s;  date -d @1700000000
来源：http://uxl.chenlongwang.top

[R71] 日期格式化
来源：http://vvf.yangfankeji.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://hcf.bjfxy.top

[R72] 等待端口就绪
来源：http://vyp.guowangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ssx.bjfxy.top

[R73] 分割大日志
来源：http://kpm.feifeiyinyue.top

split -l 1000 big.log part_
来源：http://snn.52xcode.cn

[R74] 批量重命名
来源：http://mkp.guannengcc.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://igj.shzxlz.cn

[R75] 导出环境变量
来源：http://wmg.yuxming.cn

export PATH="$HOME/bin:$PATH"
来源：http://hdp.sysykeji.top

[R76] 使用临时文件
来源：http://bhd.fzhhl.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qyo.cashguo.top

[R77] 读取用户输入
来源：http://bxz.xinyue.icu

read -rp "请输入: " ans
来源：http://zlk.yuanzhike.top

[R78] 交互式菜单
来源：http://xvm.nanxuanxn.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ipy.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://xgi.zhaomingkeji.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tva.jqgfzy.top

[R80] 查看脚本执行耗时
来源：http://fhu.bbcook.cn

time ./run.sh
来源：http://pom.dianchejie.cn

================================================================================
来源：http://gpz.shzxlz.cn

S. C / C++ 专题
来源：http://wnf.birdmap.top

================================================================================
来源：http://rtu.yj20258888.top

[S01] C：Hello World
来源：http://aiv.zhoulong.xyz

#include <stdio.h>
来源：http://ihg.0kj1m.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cym.jqgufenzy.top

[S02] C：变量与格式化输出
来源：http://kix.shanyushiyangtech.top

int a = 10; printf("%d\n", a);
来源：http://zqk.yongpay.top

[S03] C：读入整数
来源：http://hkh.vehdjk.com

int x; scanf("%d", &x);
来源：http://yuy.redwolf501.top

[S04] C：字符串复制
来源：http://nry.yj20258888.top

char dst[32]; strcpy(dst, "hi");
来源：http://pjy.dianchejie.cn

[S05] C：字符串长度
来源：http://ufj.mhx1999.top

strlen(s)
来源：http://mjt.ydjk.org.cn

[S06] C：字符串比较
来源：http://dne.zdqjudy.top

strcmp(a, b) == 0
来源：http://oya.xuanzx.com

[S07] C：数组遍历求和
来源：http://olj.ydzc1.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wnu.shanyushiyangkeji.top

[S08] C：动态内存分配与释放
来源：http://fvf.haohaochexian.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tqc.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://pec.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://avg.zhiwuduotai.top

[S10] C：指针与解引用
来源：http://rmj.iojbl.cn

int *p = &a;  *p = 5;
来源：http://xhq.sysykeji.top

[S11] C：逐行读文件
来源：http://jvp.jinqigfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://qww.svipenyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://odz.ppjwa.cn

fclose(f);
来源：http://ezt.fengsongda.top

[S12] C：写文件
来源：http://xzs.yangfankeji.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oyw.guannengcc.top

[S13] C：宏定义
来源：http://cbq.fzhhl.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dty.birdmap.top

[S14] C：枚举
来源：http://hxt.zycfv.cn

enum Color { RED, GREEN, BLUE };
来源：http://lrf.bjfxy.top

[S15] C：类型转换
来源：http://kqz.52xcode.cn

(double) a / b
来源：http://emf.hysaishi.cn

[S16] C：位操作置位
来源：http://jeh.zhoulong.xyz

x |= (1 << 3);
来源：http://ttz.hywenlv.cn

[S17] C：安全拼接字符串
来源：http://pxe.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dly.daria6918.cn

[S18] C：命令行参数
来源：http://jjx.shuidangran.top

int main(int argc, char **argv)
来源：http://wlm.ctjpmb.com

[S19] C：快速排序
来源：http://wdi.cheryme.top

qsort(a, n, sizeof(int), cmp);
来源：http://pcy.cashguo.top

[S20] C：二分查找
来源：http://ara.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ukb.chenlongwang.top

[S21] C：字符类别判断
来源：http://ksw.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://otj.fehbvm.com

[S22] C：字符串转数字
来源：http://eqz.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xbo.hongshengwenyu.top

[S23] C：随机数
来源：http://xzt.52xcode.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iyj.ppjwa.cn

[S24] C：获取本地时间
来源：http://qqn.xinyue.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uoc.sysykeji.top

[S25] C：内存拷贝
来源：http://ase.cashguo.top

memcpy(dst, src, n);
来源：http://phx.redwolf501.top

[S26] C：内存清零
来源：http://egl.hnqzz.top

memset(a, 0, sizeof a);
来源：http://xev.zycfv.cn

[S27] C：定义常量
来源：http://nss.yj20258888.top

const double PI = 3.14159;
来源：http://meo.shuidangran.top

[S28] C：静态变量
来源：http://ily.yj202588.top

static int counter = 0;
来源：http://pxk.jiagoushi.top

[S29] C：变参函数
来源：http://ezs.shangyingyoupin.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://emd.jqgufenzy.top

[S30] C：头文件保护
来源：http://jkr.fengsongda.top

#ifndef X_H
来源：http://hzq.fzhhl.top

#define X_H
来源：http://dje.yuanzhike.top

#endif
来源：http://lho.nanxinkj.top

[S31] C++：Hello World
来源：http://fdg.tarul.cn

#include <iostream>
来源：http://znh.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://zbc.hywenlv.cn

[S32] C++：字符串
来源：http://ygc.ywan-chungtsiang.top

std::string s = "hi";  s += "!";
来源：http://yqs.mhx1999.top

[S33] C++：vector 增删
来源：http://bzi.sweek.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zdt.yj202588.top

[S34] C++：遍历 vector
来源：http://tly.aibaodan.cn

for (auto &x : v) { std::cout << x; }
来源：http://grw.sysykeji.top

[S35] C++：map
来源：http://pjv.zdbjq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nmq.yvedp.cn

[S36] C++：unordered_map
来源：http://tef.ybcxt.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tnf.redwolf501.top

[S37] C++：set
来源：http://dnd.jyoumei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pvf.sxryk.cn

[S38] C++：排序
来源：http://byc.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://gep.yuxming.cn

[S39] C++：自定义比较器排序
来源：http://brk.cdnleiting.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://efk.gaohongyu789.top

[S40] C++：查找元素
来源：http://bfl.smart0.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jgy.iojbl.cn

[S41] C++：类与构造函数
来源：http://ixu.zhijiandao.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yao.nanxuanxn.top

[S42] C++：继承与虚函数
来源：http://ecw.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://rkc.yuxming.cn

[S43] C++：智能指针
来源：http://ozw.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://xlh.sxryk.cn

[S44] C++：引用传参
来源：http://its.c1oappe.top

void inc(int &x) { ++x; }
来源：http://xxt.tanke756.top

[S45] C++：lambda
来源：http://oeb.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://qtz.fehbvm.com

[S46] C++：函数模板
来源：http://rko.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uzv.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://eaf.xziqi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sja.c1oappe.top

[S48] C++：逐行读文件
来源：http://uvg.cdnleiting.top

std::ifstream in("a.txt");  std::string line;
来源：http://sse.jyoumei.cn

while (std::getline(in, line)) { }
来源：http://sja.nanxuanxn.top

[S49] C++：写文件
来源：http://znl.gaohongyu789.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lzt.wangdashe.top

[S50] C++：格式化数字
来源：http://irs.tarul.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fbx.hcnkem.com

[S51] C++：显式类型转换
来源：http://sjj.gotoacloud.top

static_cast<double>(a) / b
来源：http://vuq.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://iez.fktsv.cn

int size() const noexcept { return n_; }
来源：http://ppd.havefunace.top

[S53] C++：移动语义
来源：http://tlz.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://dft.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://btw.zhongyouzk.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gox.cucudq.cn

[S55] C++：结构化绑定
来源：http://ihn.aibaodan.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zgo.snrcjt.cn

[S56] C++：optional
来源：http://wch.cqqwz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aly.yangfankeji.com

[S57] C++：编译期常量
来源：http://cfs.yuanzhike.top

constexpr int N = 10;
来源：http://lpj.ydjk.org.cn

[S58] C++：命名空间
来源：http://vaa.ydzc1.top

namespace ns { int f() { return 1; } }
来源：http://xkg.hesvh.cn

[S59] C++：静态断言
来源：http://spi.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://btg.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://hzl.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rde.wangshuangyany.cn

================================================================================
来源：http://lkt.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://etm.gaohongyu789.top

================================================================================
来源：http://dvg.fktsv.cn

[T01] Kotlin：Hello World
来源：http://yqn.yueranfly.top

println("Hello")
来源：http://xus.0kj1m.cn

[T02] Kotlin：变量
来源：http://iyq.nanxuanxn.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lae.haohaochexian.top

[T03] Kotlin：字符串模板
来源：http://jwx.zhijiandao.cn

"值: $b"
来源：http://xge.yj20258888.top

[T04] Kotlin：空安全
来源：http://zjz.daxiang520.top

val n: String? = null;  n?.length
来源：http://mzm.shanyushiyangkeji.top

[T05] Kotlin：when 表达式
来源：http://vyg.tarul.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eit.andypj.xyz

[T06] Kotlin：集合映射
来源：http://kfu.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fer.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://dfc.vqdsnc.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fxo.redwolf501.top

[T08] Kotlin：数据类
来源：http://lha.jinyuanbaomall.cn

data class User(val name: String, val age: Int)
来源：http://uat.yangfankeji.com

[T09] Kotlin：扩展函数
来源：http://stu.xingfuxueyuan.xyz

fun String.exclaim() = this + "!"
来源：http://xho.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://uld.52xcode.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qdd.chenlongwang.top


<!-- 参考信息 -->