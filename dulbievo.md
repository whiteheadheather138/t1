代发 wailian999

case "$1" in
来源：http://vri.pycfn.com

start) echo "启动" ;;
来源：http://ywt.zhengqikj.top

stop)  echo "停止" ;;
来源：http://xxf.svipenyu.cn

*)     echo "未知命令" ;;
来源：http://hrl.ctjpmb.com

esac
来源：http://acw.hesvh.cn

[R12] for 遍历文件
来源：http://sao.aibaodan.cn

for f in *.txt; do echo "$f"; done
来源：http://snu.sufxvd.cn

[R13] for 计数循环
来源：http://ynm.guowangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://kad.cqqwz.cn

[R14] C 风格 for
来源：http://zqf.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mqa.cucudq.cn

[R15] while 逐行读文件
来源：http://ssg.yj20258.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vki.daxiang520.top

[R16] until 等待条件
来源：http://bek.0kj1m.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qlf.tian-w.cn

[R17] 数组定义与取值
来源：http://sjn.yueranfly.top

arr=(a b c); echo "${arr[0]}"
来源：http://fwc.chenjidiqi.icu

[R18] 遍历数组
来源：http://beg.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fgn.zdqjudy.top

[R19] 数组长度
来源：http://zsu.sysykeji.top

echo "${#arr[@]}"
来源：http://ueq.yonumen.top

[R20] 关联数组（字典）
来源：http://wbd.aibaodan.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xvh.wangdashe.top

[R21] 字符串长度
来源：http://snb.hcnkem.com

echo "${#s}"
来源：http://wrz.shanyushiyangtech.top

[R22] 截取子串
来源：http://qpi.shanyushiyangtech.top

echo "${s:0:5}"
来源：http://kbd.fanxiaobao.xyz

[R23] 字符串替换
来源：http://asc.dianchejie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wem.hnxiangtu.top

[R24] 大小写转换
来源：http://nxp.zdbjq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ucq.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://nqj.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://crr.sjlbkw.cn

[R26] 命令替换
来源：http://mws.chenlongwang.top

now=$(date +%F); echo "$now"
来源：http://gos.vehdjk.com

[R27] 算术展开
来源：http://ech.tian-w.cn

echo $((1 + 2 * 3))
来源：http://uae.gaohongyu789.top

[R28] 浮点运算
来源：http://hkx.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://muy.iojbl.cn

[R29] 定义函数
来源：http://cqw.zhoulong.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xse.snrcjt.cn

[R30] 函数返回状态码
来源：http://nfy.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://vvb.wangshuangyany.cn

[R31] 局部变量
来源：http://nyo.bjfxy.top

f() { local x=1; echo "$x"; }
来源：http://spf.xingfuxueyuan.xyz

[R32] 参数个数校验
来源：http://ots.yongpay.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mcj.yj20258888.top

[R33] 捕获错误并提示行号
来源：http://cqd.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ncd.fktsv.cn

[R34] 退出时清理
来源：http://ujb.epnwcf.com

trap 'rm -f "$tmp"' EXIT
来源：http://zgi.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://mit.hysaishi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rep.cqqwz.cn

[R36] 并发执行多个任务
来源：http://gdr.zhixingplan.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iac.jyoumei.cn

[R37] 把输出赋给变量
来源：http://oeb.ydjk.org.cn

files=$(ls -1)
来源：http://tty.wangshuangyany.cn

[R38] 管道串联
来源：http://wro.shuidangran.top

cat a.txt | grep -i error | wc -l
来源：http://mod.hcnkem.com

[R39] 重定向标准输出与错误
来源：http://okt.fehbvm.com

cmd > out.log 2>&1
来源：http://nqm.316326.xyz

[R40] 追加写日志
来源：http://djk.jyoumei.cn

echo "log" >> out.log
来源：http://fpk.bbcook.cn

[R41] 丢弃输出
来源：http://rox.sjlbkw.cn

cmd >/dev/null 2>&1
来源：http://aqr.cqqwz.cn

[R42] 输入重定向
来源：http://mti.zhijiandao.cn

wc -l < a.txt
来源：http://vti.zdbjq.cn

[R43] 按名字查找文件
来源：http://fsl.pengpengdd.cyou

find . -name "*.log" -type f
来源：http://kmg.yj20258888.top

[R44] 按修改时间查找
来源：http://xir.cheryme.top

find . -mtime -7 -type f
来源：http://fii.jinqigufen.top

[R45] 批量删除
来源：http://fgg.yueranfly.top

find . -name "*.tmp" -delete
来源：http://apv.c1oappe.top

[R46] 递归替换文件内容
来源：http://ran.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ayz.wangshuangyany.cn

[R47] sed 单行替换
来源：http://ufp.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://uss.tianlin.xyz

[R48] awk 取指定列
来源：http://olo.yuanzhike.top

awk '{print $1, $3}' a.txt
来源：http://osk.fktsv.cn

[R49] awk 带条件
来源：http://qhk.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dqd.nwbrower.top

[R50] awk 求和
来源：http://snk.bjfxy.top

awk '{s += $2} END {print s}' a.txt
来源：http://tkg.jqgfzy.top

[R51] 排序去重取前几
来源：http://fbr.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://ynn.epnwcf.com

[R52] 统计行数
来源：http://drv.sjlbkw.cn

wc -l a.txt
来源：http://vls.c1oappe.top

[R53] 查看文件头与实时尾
来源：http://ibk.bjfxy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ftt.yangfankeji.com

[R54] 比较两个文件
来源：http://sfa.shuidangran.top

diff a.txt b.txt
来源：http://gvc.sysykeji.top

[R55] 压缩与解压
来源：http://yqk.quarkkingdee.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jcd.jiagoushi.top

[R56] 远程拷贝
来源：http://jck.yj20258888.top

scp file user@host:/path/
来源：http://rxl.yonumen.top

[R57] 远程执行命令
来源：http://hhh.xylfe.cn

ssh user@host 'uptime'
来源：http://cph.yj20258.top

[R58] 下载文件
来源：http://gka.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tyo.yuxming.cn

[R59] 发 POST JSON
来源：http://hxz.shangyingyoupin.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ces.jyoumei.cn

[R60] 只看 HTTP 状态码
来源：http://otk.daria6918.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fjx.shuidangran.top

[R61] 磁盘占用
来源：http://ojx.aibaodan.cn

df -h;  du -sh *
来源：http://tpo.hfpthk.cn

[R62] 找最占空间的文件
来源：http://smn.yfazqb.com

du -ah . | sort -rh | head -10
来源：http://fsm.jianghu66.top

[R63] 内存与进程
来源：http://aid.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://mvr.daria6918.cn

[R64] 结束进程
来源：http://adk.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://wnm.yuanzhike.top

[R65] 查看端口占用
来源：http://psv.xziqi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uts.dianchejie.cn

[R66] 定时任务
来源：http://jdg.cashguo.top

crontab -e;  crontab -l
来源：http://btg.jianghu66.top

[R67] 生成随机十六进制串
来源：http://mlu.tian-w.cn

openssl rand -hex 16
来源：http://vnp.cqqwz.cn

[R68] 计算文件校验值
来源：http://ngj.cqqwz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tbx.birdmap.top

[R69] 生成随机密码
来源：http://rlg.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://azc.nanxinkj.top

[R70] 时间戳与互转
来源：http://txd.wangdashe.top

date +%s;  date -d @1700000000
来源：http://syi.quarkkingdee.top

[R71] 日期格式化
来源：http://kfq.ybcxt.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xhf.ydjk.org.cn

[R72] 等待端口就绪
来源：http://uvg.feifeiyinyue.top

until nc -z localhost 3306; do sleep 1; done
来源：http://soc.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://ket.ivvv.top

split -l 1000 big.log part_
来源：http://qad.zdbjq.cn

[R74] 批量重命名
来源：http://hpe.zhoulong.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://icv.fehbvm.com

[R75] 导出环境变量
来源：http://pow.wangshuangyany.cn

export PATH="$HOME/bin:$PATH"
来源：http://cjl.jinqigufen.top

[R76] 使用临时文件
来源：http://zdz.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://viy.9152youxi.cn

[R77] 读取用户输入
来源：http://lwo.zhixingplan.top

read -rp "请输入: " ans
来源：http://hyd.yj202588.top

[R78] 交互式菜单
来源：http://kln.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://imi.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://gvk.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jvy.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://gti.jlsjyb.cn

time ./run.sh
来源：http://bng.andypj.xyz

================================================================================
来源：http://kxh.shangyingyoupin.top

S. C / C++ 专题
来源：http://qad.shanyushiyangkeji.top

================================================================================
来源：http://fld.shangyingyoupin.top

[S01] C：Hello World
来源：http://sft.jinqigfzy.top

#include <stdio.h>
来源：http://pih.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pog.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://jvd.haohaochexian.top

int a = 10; printf("%d\n", a);
来源：http://xvq.mhx1999.top

[S03] C：读入整数
来源：http://xsc.xingfuxueyuan.xyz

int x; scanf("%d", &x);
来源：http://jme.yongpay.top

[S04] C：字符串复制
来源：http://uaw.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://klp.xuanzx.com

[S05] C：字符串长度
来源：http://nkw.shuidangran.top

strlen(s)
来源：http://kws.hywenlv.cn

[S06] C：字符串比较
来源：http://eus.redwolf501.top

strcmp(a, b) == 0
来源：http://zaq.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://rtn.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cml.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://isf.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yvy.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://yhp.guannengcc.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wyy.xinyue.icu

[S10] C：指针与解引用
来源：http://rim.havefunace.top

int *p = &a;  *p = 5;
来源：http://dar.tarul.cn

[S11] C：逐行读文件
来源：http://xmb.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://yfw.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eed.jianghu66.top

fclose(f);
来源：http://swp.xuetiantiany.cn

[S12] C：写文件
来源：http://gef.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nqy.guowangkeji.top

[S13] C：宏定义
来源：http://vpt.chenlongwang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bqt.gogol.net.cn

[S14] C：枚举
来源：http://qtx.hfpthk.cn

enum Color { RED, GREEN, BLUE };
来源：http://ger.gaohongyu789.top

[S15] C：类型转换
来源：http://tkj.svipenyu.cn

(double) a / b
来源：http://mcd.guowangkeji.top

[S16] C：位操作置位
来源：http://dfk.chenlongwang.top

x |= (1 << 3);
来源：http://old.316326.xyz

[S17] C：安全拼接字符串
来源：http://dod.tanke756.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dfn.quarkkingdee.top

[S18] C：命令行参数
来源：http://dky.vqdsnc.cn

int main(int argc, char **argv)
来源：http://pif.yongpay.top

[S19] C：快速排序
来源：http://nlx.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ekr.yangfankeji.com

[S20] C：二分查找
来源：http://iwj.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fsi.fanxiaobao.xyz

[S21] C：字符类别判断
来源：http://pqg.jinqigufen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vyf.dianchejie.cn

[S22] C：字符串转数字
来源：http://ydf.uphjek.com

atoi("42");  strtod("3.14", NULL);
来源：http://jne.quarkkingdee.top

[S23] C：随机数
来源：http://pgr.tanke756.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cdk.yvedp.cn

[S24] C：获取本地时间
来源：http://vmp.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ynz.yj202588.top

[S25] C：内存拷贝
来源：http://agu.zhongyouzk.top

memcpy(dst, src, n);
来源：http://hss.yanxiufei.cn

[S26] C：内存清零
来源：http://qru.fktsv.cn

memset(a, 0, sizeof a);
来源：http://yzi.yonumen.top

[S27] C：定义常量
来源：http://zro.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://rsj.gogol.net.cn

[S28] C：静态变量
来源：http://zpe.bjfxy.top

static int counter = 0;
来源：http://del.yvedp.cn

[S29] C：变参函数
来源：http://ajk.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ajx.yvedp.cn

[S30] C：头文件保护
来源：http://mmm.zdqjudy.top

#ifndef X_H
来源：http://woz.ctjpmb.com

#define X_H
来源：http://iws.iojbl.cn

#endif
来源：http://lxc.sysykeji.top

[S31] C++：Hello World
来源：http://vrm.kuanghao11.cn

#include <iostream>
来源：http://obc.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://ami.yuanzhike.top

[S32] C++：字符串
来源：http://kkd.yj202588.top

std::string s = "hi";  s += "!";
来源：http://azs.xinyue.icu

[S33] C++：vector 增删
来源：http://ytl.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://onw.xziqi.cn

[S34] C++：遍历 vector
来源：http://tuu.nanxinkj.top

for (auto &x : v) { std::cout << x; }
来源：http://orr.bjfxy.top

[S35] C++：map
来源：http://gfu.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rrj.jqgfzy.top

[S36] C++：unordered_map
来源：http://jkw.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hvw.zycfv.cn

[S37] C++：set
来源：http://sxg.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://txl.yj20258888.top

[S38] C++：排序
来源：http://sta.yj20258.top

std::sort(v.begin(), v.end());
来源：http://zfr.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://opr.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tvr.jqgfzy.top

[S40] C++：查找元素
来源：http://pox.jqgfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vox.sjlbkw.cn

[S41] C++：类与构造函数
来源：http://ksv.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://feh.yvedp.cn

[S42] C++：继承与虚函数
来源：http://axi.hywenlv.cn

class B : public Base { public: void f() override {} };
来源：http://yir.zhiwuduotai.top

[S43] C++：智能指针
来源：http://kcg.jinqigfzy.top

auto p = std::make_unique<int>(5);
来源：http://pnx.shanyushiyangtech.top

[S44] C++：引用传参
来源：http://awk.wangdashe.top

void inc(int &x) { ++x; }
来源：http://ogu.9152youxi.cn

[S45] C++：lambda
来源：http://egw.yj202588.top

auto add = [](int a, int b) { return a + b; };
来源：http://lvw.jinqigufen.top

[S46] C++：函数模板
来源：http://dsu.zhijiandao.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zdk.gotoacloud.top

[S47] C++：结构化绑定遍历
来源：http://doy.tianlin.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gwl.zycfv.cn

[S48] C++：逐行读文件
来源：http://avh.sjlbkw.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oyr.jiagoushi.top

while (std::getline(in, line)) { }
来源：http://vap.pengpengdd.cyou

[S49] C++：写文件
来源：http://vuz.gaohongyu789.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lwq.hnxiangtu.top

[S50] C++：格式化数字
来源：http://hfc.shanyushiyangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kuu.fehbvm.com

[S51] C++：显式类型转换
来源：http://rkj.xuanzx.com

static_cast<double>(a) / b
来源：http://drc.dashuyun.cn

[S52] C++：const 与 noexcept
来源：http://scu.fktsv.cn

int size() const noexcept { return n_; }
来源：http://gba.aibaodan.cn

[S53] C++：移动语义
来源：http://rwu.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://tym.jianghu66.top

[S54] C++：异常处理
来源：http://eml.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dfp.yj20258.top

[S55] C++：结构化绑定
来源：http://nay.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gvx.ehwqpu.com

[S56] C++：optional
来源：http://nwq.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dkl.uphjek.com

[S57] C++：编译期常量
来源：http://brf.zhijiandao.cn

constexpr int N = 10;
来源：http://hha.fengsongda.top

[S58] C++：命名空间
来源：http://wvc.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://tbb.yj20258.top

[S59] C++：静态断言
来源：http://duu.daxiang520.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rsu.jyoumei.cn

[S60] C++：遍历并删除元素
来源：http://nms.pycfn.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ayd.andypj.xyz

================================================================================
来源：http://ylu.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rmq.ydzc1.top

================================================================================
来源：http://uzw.yj20258888.top

[T01] Kotlin：Hello World
来源：http://wpw.jinghuilouyu.cn

println("Hello")
来源：http://shv.quarkkingdee.top

[T02] Kotlin：变量
来源：http://zwz.jinqigufen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iif.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://huv.quarkkingdee.top

"值: $b"
来源：http://fna.jianghu66.top

[T04] Kotlin：空安全
来源：http://qkh.dashuyun.cn

val n: String? = null;  n?.length
来源：http://pjt.bjfxy.top

[T05] Kotlin：when 表达式
来源：http://gls.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kmw.nanxuanxn.top

[T06] Kotlin：集合映射
来源：http://aqh.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lup.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://jpl.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fif.meibo888.top

[T08] Kotlin：数据类
来源：http://aib.birdmap.top

data class User(val name: String, val age: Int)
来源：http://drx.uphjek.com

[T09] Kotlin：扩展函数
来源：http://lmc.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://weo.fzhhl.top

[T10] Kotlin：默认参数
来源：http://nlz.ydjk.org.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jqi.sjlbkw.cn

[T11] Kotlin：协程
来源：http://dov.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ylg.jqgufenzy.top

[T12] Kotlin：解构声明
来源：http://lyk.yvedp.cn

val (a, b) = Pair(1, 2)
来源：http://ibn.shangyingyoupin.top


<!-- 参考信息 -->