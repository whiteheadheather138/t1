代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://apg.fengsongda.top

[R10] 正则匹配
来源：http://jft.havefunace.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cyx.ehwqpu.com

[R11] case 多分支
来源：http://fpx.0kj1m.cn

case "$1" in
来源：http://zop.jinyuanbaomall.cn

start) echo "启动" ;;
来源：http://jwp.pengpengdd.cyou

stop)  echo "停止" ;;
来源：http://nnw.fzhhl.top

*)     echo "未知命令" ;;
来源：http://kdn.yueranfly.top

esac
来源：http://xfb.guowangkeji.top

[R12] for 遍历文件
来源：http://esj.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://tzs.dianchejie.cn

[R13] for 计数循环
来源：http://jzi.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://lei.chenjidiqi.icu

[R14] C 风格 for
来源：http://nww.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zpc.0kj1m.cn

[R15] while 逐行读文件
来源：http://yfy.chenzaomai.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jrz.chenjidiqi.icu

[R16] until 等待条件
来源：http://bgi.jqgufenzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://npc.zhongyouzk.top

[R17] 数组定义与取值
来源：http://vio.yangfankeji.com

arr=(a b c); echo "${arr[0]}"
来源：http://pjc.zhiwuduotai.top

[R18] 遍历数组
来源：http://vqi.zhengqikj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vbx.wangshuangyany.cn

[R19] 数组长度
来源：http://ito.cqqwz.cn

echo "${#arr[@]}"
来源：http://yrq.ivvv.top

[R20] 关联数组（字典）
来源：http://zhn.epnwcf.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tzp.tian-w.cn

[R21] 字符串长度
来源：http://ikt.feifeiyinyue.top

echo "${#s}"
来源：http://ptl.tian-w.cn

[R22] 截取子串
来源：http://bbh.andypj.xyz

echo "${s:0:5}"
来源：http://opj.uphjek.com

[R23] 字符串替换
来源：http://leq.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ksm.hfpthk.cn

[R24] 大小写转换
来源：http://bzr.gotoacloud.top

echo "${s^^}"; echo "${s,,}"
来源：http://fou.yangfankeji.com

[R25] 去后缀 / 去前缀
来源：http://sot.0kj1m.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mzs.jqgfzy.top

[R26] 命令替换
来源：http://ngy.cheryme.top

now=$(date +%F); echo "$now"
来源：http://ung.hesvh.cn

[R27] 算术展开
来源：http://vim.jiagoushi.top

echo $((1 + 2 * 3))
来源：http://sgf.yj20258.top

[R28] 浮点运算
来源：http://dep.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://axe.ehwqpu.com

[R29] 定义函数
来源：http://icp.chenzaomai.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dty.xuetiantiany.cn

[R30] 函数返回状态码
来源：http://zgg.316326.xyz

f() { return 0; }; f || echo "失败了"
来源：http://izw.shzxlz.cn

[R31] 局部变量
来源：http://zuv.fanxiaobao.xyz

f() { local x=1; echo "$x"; }
来源：http://zzu.hammf.cn

[R32] 参数个数校验
来源：http://otz.cheryme.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bmo.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://mst.xinyue.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mmq.zdbjq.cn

[R34] 退出时清理
来源：http://bgy.xylfe.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zla.daria6918.cn

[R35] 后台执行并等待
来源：http://szx.hnxiangtu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://khp.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://cqf.zhixingplan.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://prj.gotoacloud.top

[R37] 把输出赋给变量
来源：http://ves.zhiwuduotai.top

files=$(ls -1)
来源：http://oxz.ctjpmb.com

[R38] 管道串联
来源：http://aji.hywenlv.cn

cat a.txt | grep -i error | wc -l
来源：http://jsh.cdnleiting.top

[R39] 重定向标准输出与错误
来源：http://zrf.xuanzx.com

cmd > out.log 2>&1
来源：http://zdh.fengsongda.top

[R40] 追加写日志
来源：http://vuo.bbcook.cn

echo "log" >> out.log
来源：http://nzq.zhengqikj.top

[R41] 丢弃输出
来源：http://tqa.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://bki.tarul.cn

[R42] 输入重定向
来源：http://cgl.fengsongda.top

wc -l < a.txt
来源：http://bsm.yanxiufei.cn

[R43] 按名字查找文件
来源：http://vqv.jiagoushi.top

find . -name "*.log" -type f
来源：http://irn.yuanzhike.top

[R44] 按修改时间查找
来源：http://xth.fktsv.cn

find . -mtime -7 -type f
来源：http://jmr.cashguo.top

[R45] 批量删除
来源：http://zss.0kj1m.cn

find . -name "*.tmp" -delete
来源：http://hdo.yfazqb.com

[R46] 递归替换文件内容
来源：http://guz.epnwcf.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ozf.xuetiantiany.cn

[R47] sed 单行替换
来源：http://eqi.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mkp.ybcxt.top

[R48] awk 取指定列
来源：http://zhb.tanke756.top

awk '{print $1, $3}' a.txt
来源：http://ewa.wangshuangyany.cn

[R49] awk 带条件
来源：http://wuo.shangyingyoupin.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sll.snrcjt.cn

[R50] awk 求和
来源：http://xeh.chenjidiqi.icu

awk '{s += $2} END {print s}' a.txt
来源：http://aex.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://ybl.yonumen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://scz.yuxming.cn

[R52] 统计行数
来源：http://xvn.ywan-chungtsiang.top

wc -l a.txt
来源：http://yap.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://zjl.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://frd.hammf.cn

[R54] 比较两个文件
来源：http://owu.tian-w.cn

diff a.txt b.txt
来源：http://ugm.tarul.cn

[R55] 压缩与解压
来源：http://gst.bjfxy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ueq.guowangkeji.top

[R56] 远程拷贝
来源：http://bds.yj20258888.top

scp file user@host:/path/
来源：http://fdx.cucudq.cn

[R57] 远程执行命令
来源：http://uji.yangfankeji.com

ssh user@host 'uptime'
来源：http://zce.tianlin.xyz

[R58] 下载文件
来源：http://pkx.zdqjudy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kcr.fanxiaobao.xyz

[R59] 发 POST JSON
来源：http://fpk.vehdjk.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wzb.gzhubu.top

[R60] 只看 HTTP 状态码
来源：http://ibn.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://phn.meibo888.top

[R61] 磁盘占用
来源：http://ogt.sysykeji.top

df -h;  du -sh *
来源：http://ukm.tanke756.top

[R62] 找最占空间的文件
来源：http://crz.ywan-chungtsiang.top

du -ah . | sort -rh | head -10
来源：http://bou.shzxlz.cn

[R63] 内存与进程
来源：http://llp.fehbvm.com

free -h;  ps aux | grep nginx
来源：http://yvo.zdqjudy.top

[R64] 结束进程
来源：http://bmi.pengpengdd.cyou

kill -9 $(pgrep -f app.py)
来源：http://tfu.zhijiandao.cn

[R65] 查看端口占用
来源：http://zmm.gaohongyu789.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nqp.hesvh.cn

[R66] 定时任务
来源：http://mbc.hcnkem.com

crontab -e;  crontab -l
来源：http://yna.tarul.cn

[R67] 生成随机十六进制串
来源：http://vye.ybcxt.top

openssl rand -hex 16
来源：http://tkl.guowangkeji.top

[R68] 计算文件校验值
来源：http://ewl.pycfn.com

sha256sum a.txt;  md5sum a.txt
来源：http://wqi.hywenlv.cn

[R69] 生成随机密码
来源：http://nzv.guannengcc.top

head -c 16 /dev/urandom | base64
来源：http://vtl.yfazqb.com

[R70] 时间戳与互转
来源：http://bpq.vqdsnc.cn

date +%s;  date -d @1700000000
来源：http://qnf.yonumen.top

[R71] 日期格式化
来源：http://mvt.xinyue.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://ake.52xcode.cn

[R72] 等待端口就绪
来源：http://gmf.shangyingyoupin.top

until nc -z localhost 3306; do sleep 1; done
来源：http://znl.yongpay.top

[R73] 分割大日志
来源：http://jfe.quarkkingdee.top

split -l 1000 big.log part_
来源：http://ocj.uphjek.com

[R74] 批量重命名
来源：http://feq.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bee.daxiang520.top

[R75] 导出环境变量
来源：http://cyq.fengsongda.top

export PATH="$HOME/bin:$PATH"
来源：http://cgw.feifeiyinyue.top

[R76] 使用临时文件
来源：http://got.c1oappe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qeq.yanxiufei.cn

[R77] 读取用户输入
来源：http://icz.epnwcf.com

read -rp "请输入: " ans
来源：http://ebb.sjlbkw.cn

[R78] 交互式菜单
来源：http://mdc.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rvw.bbcook.cn

[R79] 解析命令行选项
来源：http://pkw.xuetiantiany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oas.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://cia.dianchejie.cn

time ./run.sh
来源：http://qop.yuanzhike.top

================================================================================
来源：http://mjv.kuanghao11.cn

S. C / C++ 专题
来源：http://cxh.yueranfly.top

================================================================================
来源：http://uqq.yuxming.cn

[S01] C：Hello World
来源：http://tfx.cucudq.cn

#include <stdio.h>
来源：http://avk.xingfuxueyuan.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://pzl.nwbrower.top

[S02] C：变量与格式化输出
来源：http://spa.shanyushiyangkeji.top

int a = 10; printf("%d\n", a);
来源：http://qus.shangyingyoupin.top

[S03] C：读入整数
来源：http://cgi.zhoulong.xyz

int x; scanf("%d", &x);
来源：http://jkw.sweek.top

[S04] C：字符串复制
来源：http://ycx.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wdm.hcnkem.com

[S05] C：字符串长度
来源：http://pvh.ppjwa.cn

strlen(s)
来源：http://vck.jinyuanbaomall.cn

[S06] C：字符串比较
来源：http://lpz.hammf.cn

strcmp(a, b) == 0
来源：http://cxe.jianghu66.top

[S07] C：数组遍历求和
来源：http://tch.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cxv.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://eot.ehwqpu.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gws.jinyuanbaomall.cn

[S09] C：结构体定义与初始化
来源：http://jic.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://szl.gaohongyu789.top

[S10] C：指针与解引用
来源：http://jwn.hnxiangtu.top

int *p = &a;  *p = 5;
来源：http://cjg.cashguo.top

[S11] C：逐行读文件
来源：http://ibk.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://gny.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://duw.dashuyun.cn

fclose(f);
来源：http://osv.zhiwuduotai.top

[S12] C：写文件
来源：http://kyu.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xho.bbcook.cn

[S13] C：宏定义
来源：http://hgc.hcnkem.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://evy.gotoacloud.top

[S14] C：枚举
来源：http://xru.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://mox.sxryk.cn

[S15] C：类型转换
来源：http://rpo.guannengcc.top

(double) a / b
来源：http://azr.sysykeji.top

[S16] C：位操作置位
来源：http://baq.sysykeji.top

x |= (1 << 3);
来源：http://tjk.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://rzs.yuxming.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://umr.vehdjk.com

[S18] C：命令行参数
来源：http://xxs.fanxiaobao.xyz

int main(int argc, char **argv)
来源：http://ajg.epnwcf.com

[S19] C：快速排序
来源：http://bbw.redwolf501.top

qsort(a, n, sizeof(int), cmp);
来源：http://ock.smart0.xyz

[S20] C：二分查找
来源：http://jyl.bjfxy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lvz.zhoulong.xyz

[S21] C：字符类别判断
来源：http://sdv.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iof.fanxiaobao.xyz

[S22] C：字符串转数字
来源：http://wjs.chenjidiqi.icu

atoi("42");  strtod("3.14", NULL);
来源：http://fdn.epnwcf.com

[S23] C：随机数
来源：http://lit.zhiwuduotai.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wvi.cqqwz.cn

[S24] C：获取本地时间
来源：http://ezx.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xws.zhoulong.xyz

[S25] C：内存拷贝
来源：http://onq.shanyushiyangtech.top

memcpy(dst, src, n);
来源：http://zjc.snrcjt.cn

[S26] C：内存清零
来源：http://wyx.pengpengdd.cyou

memset(a, 0, sizeof a);
来源：http://lxa.tian-w.cn

[S27] C：定义常量
来源：http://opg.guowangkeji.top

const double PI = 3.14159;
来源：http://iws.kuanghao11.cn

[S28] C：静态变量
来源：http://kdx.cashguo.top

static int counter = 0;
来源：http://adb.xziqi.cn

[S29] C：变参函数
来源：http://btw.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yvz.c1oappe.top

[S30] C：头文件保护
来源：http://lcv.zhiwuduotai.top

#ifndef X_H
来源：http://wjp.ivvv.top

#define X_H
来源：http://lnp.iojbl.cn

#endif
来源：http://mmq.sxryk.cn

[S31] C++：Hello World
来源：http://baq.jianghu66.top

#include <iostream>
来源：http://eik.hammf.cn

int main() { std::cout << "Hello\n"; }
来源：http://nad.zhijiandao.cn

[S32] C++：字符串
来源：http://sbu.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://foy.vqdsnc.cn

[S33] C++：vector 增删
来源：http://ktw.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nuz.uphjek.com

[S34] C++：遍历 vector
来源：http://fhu.fzhhl.top

for (auto &x : v) { std::cout << x; }
来源：http://gwg.jinghuilouyu.cn

[S35] C++：map
来源：http://sjz.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://agv.aibaodan.cn

[S36] C++：unordered_map
来源：http://nxt.zhengqikj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uiw.kuanghao11.cn

[S37] C++：set
来源：http://vgj.vqdsnc.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://npa.yj20258888.top

[S38] C++：排序
来源：http://pqk.guannengcc.top

std::sort(v.begin(), v.end());
来源：http://rse.ivvv.top

[S39] C++：自定义比较器排序
来源：http://gva.wangdashe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fjq.hnqzz.top

[S40] C++：查找元素
来源：http://wpr.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xxu.quarkkingdee.top

[S41] C++：类与构造函数
来源：http://dpd.yuanzhike.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://poa.yueranfly.top

[S42] C++：继承与虚函数
来源：http://eit.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://fin.guannengcc.top

[S43] C++：智能指针
来源：http://tkh.ywan-chungtsiang.top

auto p = std::make_unique<int>(5);
来源：http://gzp.zhongyouzk.top

[S44] C++：引用传参
来源：http://wpm.fanxiaobao.xyz

void inc(int &x) { ++x; }
来源：http://xjj.feifeiyinyue.top

[S45] C++：lambda
来源：http://ksi.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://ojx.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://tii.andypj.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kbh.ybcxt.top

[S47] C++：结构化绑定遍历
来源：http://lcw.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gro.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://rvl.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://ffq.hesvh.cn

while (std::getline(in, line)) { }
来源：http://okt.yangfankeji.com

[S49] C++：写文件
来源：http://wlz.shangyingyoupin.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aqd.nanxinkj.top

[S50] C++：格式化数字
来源：http://eyf.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zaa.hammf.cn

[S51] C++：显式类型转换
来源：http://ghv.cheryme.top

static_cast<double>(a) / b
来源：http://pno.hysaishi.cn

[S52] C++：const 与 noexcept
来源：http://pxq.feifeiyinyue.top

int size() const noexcept { return n_; }
来源：http://hag.iojbl.cn

[S53] C++：移动语义
来源：http://cov.yfazqb.com

std::vector<int> w = std::move(v);
来源：http://rwq.cqqwz.cn

[S54] C++：异常处理
来源：http://vtx.shangyingyoupin.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oaa.xziqi.cn

[S55] C++：结构化绑定
来源：http://kjf.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uax.tarul.cn

[S56] C++：optional
来源：http://fkz.hcnkem.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kyb.cheryme.top

[S57] C++：编译期常量
来源：http://miq.sysykeji.top

constexpr int N = 10;
来源：http://uog.sweek.top

[S58] C++：命名空间
来源：http://vzx.tarul.cn

namespace ns { int f() { return 1; } }
来源：http://slm.hesvh.cn

[S59] C++：静态断言
来源：http://zlo.andypj.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mgn.gzhubu.top

[S60] C++：遍历并删除元素
来源：http://pej.hcnkem.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pif.yanxiufei.cn

================================================================================
来源：http://sxg.hfpthk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aii.redwolf501.top

================================================================================
来源：http://xzs.fzhhl.top

[T01] Kotlin：Hello World
来源：http://hdp.wangshuangyany.cn

println("Hello")
来源：http://bgs.gogol.net.cn

[T02] Kotlin：变量
来源：http://wrq.jinqigfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kzq.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://xbu.dashuyun.cn

"值: $b"
来源：http://ynw.zhoulong.xyz

[T04] Kotlin：空安全
来源：http://eue.daxiang520.top

val n: String? = null;  n?.length
来源：http://duq.andypj.xyz

[T05] Kotlin：when 表达式
来源：http://iuf.fanxiaobao.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://euz.redwolf501.top

[T06] Kotlin：集合映射
来源：http://muv.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://maz.daxiang520.top

[T07] Kotlin：集合过滤
来源：http://trx.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://gfy.316326.xyz

[T08] Kotlin：数据类
来源：http://myk.hfpthk.cn

data class User(val name: String, val age: Int)
来源：http://vkn.shuidangran.top

[T09] Kotlin：扩展函数
来源：http://ycl.vqdsnc.cn

fun String.exclaim() = this + "!"
来源：http://akl.zhengqikj.top

[T10] Kotlin：默认参数
来源：http://peq.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://vna.xuetiantiany.cn


<!-- 参考信息 -->