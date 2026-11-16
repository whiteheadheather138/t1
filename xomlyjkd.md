代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cjv.yanxiufei.cn

[R08] 数值比较
来源：http://jsm.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://odn.fengsongda.top

[R09] 字符串比较
来源：http://pjw.ppjwa.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fsd.chenzaomai.com

[R10] 正则匹配
来源：http://lzb.birdmap.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kww.chenlongwang.top

[R11] case 多分支
来源：http://juv.9152youxi.cn

case "$1" in
来源：http://hsu.pycfn.com

start) echo "启动" ;;
来源：http://hwt.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://epd.nwbrower.top

*)     echo "未知命令" ;;
来源：http://gam.fengsongda.top

esac
来源：http://fkq.xziqi.cn

[R12] for 遍历文件
来源：http://ngu.ydjk.org.cn

for f in *.txt; do echo "$f"; done
来源：http://hah.xuanzx.com

[R13] for 计数循环
来源：http://ymz.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://gxm.hammf.cn

[R14] C 风格 for
来源：http://yht.fanxiaobao.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uhc.sufxvd.cn

[R15] while 逐行读文件
来源：http://ybw.sufxvd.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gqb.zhiwuduotai.top

[R16] until 等待条件
来源：http://pyl.ivvv.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dgx.ybcxt.top

[R17] 数组定义与取值
来源：http://acr.hnqzz.top

arr=(a b c); echo "${arr[0]}"
来源：http://xaz.uphjek.com

[R18] 遍历数组
来源：http://yms.fengsongda.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ybu.fzhhl.top

[R19] 数组长度
来源：http://bwn.jyoumei.cn

echo "${#arr[@]}"
来源：http://obd.nwbrower.top

[R20] 关联数组（字典）
来源：http://rgf.zycfv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tad.sweek.top

[R21] 字符串长度
来源：http://tvg.9152youxi.cn

echo "${#s}"
来源：http://acy.wangshuangyany.cn

[R22] 截取子串
来源：http://vmh.tianlin.xyz

echo "${s:0:5}"
来源：http://xdq.yj202588.top

[R23] 字符串替换
来源：http://xgn.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ted.hysaishi.cn

[R24] 大小写转换
来源：http://pcq.zhijiandao.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tpa.mhx1999.top

[R25] 去后缀 / 去前缀
来源：http://brd.jqgfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ahr.sysykeji.top

[R26] 命令替换
来源：http://hrd.vehdjk.com

now=$(date +%F); echo "$now"
来源：http://efl.jqgfzy.top

[R27] 算术展开
来源：http://mne.sufxvd.cn

echo $((1 + 2 * 3))
来源：http://ufh.yonumen.top

[R28] 浮点运算
来源：http://asn.fengsongda.top

echo "scale=2; 10/3" | bc
来源：http://qnk.hfpthk.cn

[R29] 定义函数
来源：http://oep.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qen.nanxinkj.top

[R30] 函数返回状态码
来源：http://aom.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://wkh.nwbrower.top

[R31] 局部变量
来源：http://waa.316326.xyz

f() { local x=1; echo "$x"; }
来源：http://fbm.gzhubu.top

[R32] 参数个数校验
来源：http://oqk.ppjwa.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zcv.zhongyouzk.top

[R33] 捕获错误并提示行号
来源：http://vgy.hywenlv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eaa.jlsjyb.cn

[R34] 退出时清理
来源：http://bns.pengpengdd.cyou

trap 'rm -f "$tmp"' EXIT
来源：http://ghh.ydzc1.top

[R35] 后台执行并等待
来源：http://trc.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://itz.hcnkem.com

[R36] 并发执行多个任务
来源：http://cgt.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://has.havefunace.top

[R37] 把输出赋给变量
来源：http://qjz.yfazqb.com

files=$(ls -1)
来源：http://uko.sxryk.cn

[R38] 管道串联
来源：http://ewx.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://ozx.daria6918.cn

[R39] 重定向标准输出与错误
来源：http://cjg.ydzc1.top

cmd > out.log 2>&1
来源：http://nnn.fengsongda.top

[R40] 追加写日志
来源：http://vkh.c1oappe.top

echo "log" >> out.log
来源：http://snl.guowangkeji.top

[R41] 丢弃输出
来源：http://jcr.jinqigufen.top

cmd >/dev/null 2>&1
来源：http://fil.xuanzx.com

[R42] 输入重定向
来源：http://ukz.birdmap.top

wc -l < a.txt
来源：http://pik.andypj.xyz

[R43] 按名字查找文件
来源：http://aey.zhongyouzk.top

find . -name "*.log" -type f
来源：http://qcs.zycfv.cn

[R44] 按修改时间查找
来源：http://iux.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://khl.zhaomingkeji.xyz

[R45] 批量删除
来源：http://rdo.vehdjk.com

find . -name "*.tmp" -delete
来源：http://tgd.sufxvd.cn

[R46] 递归替换文件内容
来源：http://ugb.yongpay.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zke.hammf.cn

[R47] sed 单行替换
来源：http://zxw.hywenlv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nqo.ywan-chungtsiang.top

[R48] awk 取指定列
来源：http://xzk.xinyue.icu

awk '{print $1, $3}' a.txt
来源：http://zci.zdqjudy.top

[R49] awk 带条件
来源：http://jgt.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pur.havefunace.top

[R50] awk 求和
来源：http://ypb.wangdashe.top

awk '{s += $2} END {print s}' a.txt
来源：http://kbl.dianchejie.cn

[R51] 排序去重取前几
来源：http://tgv.xziqi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zfz.zdqjudy.top

[R52] 统计行数
来源：http://iln.cucudq.cn

wc -l a.txt
来源：http://thl.ydjk.org.cn

[R53] 查看文件头与实时尾
来源：http://ket.xuanzx.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://com.ivvv.top

[R54] 比较两个文件
来源：http://vzq.nanxuanxn.top

diff a.txt b.txt
来源：http://zva.hesvh.cn

[R55] 压缩与解压
来源：http://fpv.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mrf.vqdsnc.cn

[R56] 远程拷贝
来源：http://odf.chenjidiqi.icu

scp file user@host:/path/
来源：http://mql.zhongyouzk.top

[R57] 远程执行命令
来源：http://vec.jianghu66.top

ssh user@host 'uptime'
来源：http://zxj.fktsv.cn

[R58] 下载文件
来源：http://ugi.hysaishi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vwy.shanyushiyangtech.top

[R59] 发 POST JSON
来源：http://ona.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zam.gogol.net.cn

[R60] 只看 HTTP 状态码
来源：http://olh.c1oappe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kns.zhoulong.xyz

[R61] 磁盘占用
来源：http://idv.zdbjq.cn

df -h;  du -sh *
来源：http://jot.birdmap.top

[R62] 找最占空间的文件
来源：http://kpe.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://mpr.mhx1999.top

[R63] 内存与进程
来源：http://dnw.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://xih.fengsongda.top

[R64] 结束进程
来源：http://ipa.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://sex.zhongyouzk.top

[R65] 查看端口占用
来源：http://uhu.ehwqpu.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kus.pycfn.com

[R66] 定时任务
来源：http://kdw.daxiang520.top

crontab -e;  crontab -l
来源：http://wpn.hnqzz.top

[R67] 生成随机十六进制串
来源：http://fni.hysaishi.cn

openssl rand -hex 16
来源：http://ajj.ctjpmb.com

[R68] 计算文件校验值
来源：http://nin.shangyingyoupin.top

sha256sum a.txt;  md5sum a.txt
来源：http://jtg.fehbvm.com

[R69] 生成随机密码
来源：http://hzy.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://gtr.jiagoushi.top

[R70] 时间戳与互转
来源：http://udh.zhoulong.xyz

date +%s;  date -d @1700000000
来源：http://kwh.shzxlz.cn

[R71] 日期格式化
来源：http://fwu.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rpq.chenlongwang.top

[R72] 等待端口就绪
来源：http://vmb.gzhubu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bmz.yuanzhike.top

[R73] 分割大日志
来源：http://nfk.zhengqikj.top

split -l 1000 big.log part_
来源：http://iix.cashguo.top

[R74] 批量重命名
来源：http://ats.chenjidiqi.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://adv.sxryk.cn

[R75] 导出环境变量
来源：http://bem.feifeiyinyue.top

export PATH="$HOME/bin:$PATH"
来源：http://osi.shuidangran.top

[R76] 使用临时文件
来源：http://thr.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yxs.gogol.net.cn

[R77] 读取用户输入
来源：http://mif.zhijiandao.cn

read -rp "请输入: " ans
来源：http://ndj.tanke756.top

[R78] 交互式菜单
来源：http://pbv.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ezf.tarul.cn

[R79] 解析命令行选项
来源：http://bwt.chenlongwang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gsu.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://bjx.hesvh.cn

time ./run.sh
来源：http://mmd.yj202588.top

================================================================================
来源：http://wyy.ydjk.org.cn

S. C / C++ 专题
来源：http://rha.birdmap.top

================================================================================
来源：http://sjd.guannengcc.top

[S01] C：Hello World
来源：http://elm.ppjwa.cn

#include <stdio.h>
来源：http://dsd.chenzaomai.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://bla.cqqwz.cn

[S02] C：变量与格式化输出
来源：http://csr.ydjk.org.cn

int a = 10; printf("%d\n", a);
来源：http://baa.aibaodan.cn

[S03] C：读入整数
来源：http://dko.redwolf501.top

int x; scanf("%d", &x);
来源：http://aze.jinqigufen.top

[S04] C：字符串复制
来源：http://maz.zhijiandao.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vvb.tianlin.xyz

[S05] C：字符串长度
来源：http://vjp.ctjpmb.com

strlen(s)
来源：http://zuu.ehwqpu.com

[S06] C：字符串比较
来源：http://gxr.ppjwa.cn

strcmp(a, b) == 0
来源：http://gkk.cqqwz.cn

[S07] C：数组遍历求和
来源：http://nni.ctjpmb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bcv.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://efy.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iss.zdqjudy.top

[S09] C：结构体定义与初始化
来源：http://jwh.haohaochexian.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aov.kuanghao11.cn

[S10] C：指针与解引用
来源：http://tcv.xylfe.cn

int *p = &a;  *p = 5;
来源：http://brd.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://ork.pengpengdd.cyou

FILE *f = fopen("a.txt", "r");
来源：http://jfl.hysaishi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qow.epnwcf.com

fclose(f);
来源：http://twf.nwbrower.top

[S12] C：写文件
来源：http://zua.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://drq.jqgufenzy.top

[S13] C：宏定义
来源：http://nsn.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yro.zhiwuduotai.top

[S14] C：枚举
来源：http://dkr.jianghu66.top

enum Color { RED, GREEN, BLUE };
来源：http://nwj.nanxinkj.top

[S15] C：类型转换
来源：http://luh.hongshengwenyu.top

(double) a / b
来源：http://xqi.sysykeji.top

[S16] C：位操作置位
来源：http://jwg.shuidangran.top

x |= (1 << 3);
来源：http://cdv.nwbrower.top

[S17] C：安全拼接字符串
来源：http://nsh.shzxlz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xfr.bjfxy.top

[S18] C：命令行参数
来源：http://ijx.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://zfw.guowangkeji.top

[S19] C：快速排序
来源：http://dvn.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://cbs.fktsv.cn

[S20] C：二分查找
来源：http://ved.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://chl.zhengqikj.top

[S21] C：字符类别判断
来源：http://cyv.zhixingplan.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zaq.zycfv.cn

[S22] C：字符串转数字
来源：http://wra.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tdz.xinyue.icu

[S23] C：随机数
来源：http://tex.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oca.chenjidiqi.icu

[S24] C：获取本地时间
来源：http://cvy.feifeiyinyue.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ool.feifeiyinyue.top

[S25] C：内存拷贝
来源：http://rvl.jqgufenzy.top

memcpy(dst, src, n);
来源：http://riq.shzxlz.cn

[S26] C：内存清零
来源：http://vnq.redwolf501.top

memset(a, 0, sizeof a);
来源：http://cgv.shzxlz.cn

[S27] C：定义常量
来源：http://lao.svipenyu.cn

const double PI = 3.14159;
来源：http://zpr.hammf.cn

[S28] C：静态变量
来源：http://hri.jinqigufen.top

static int counter = 0;
来源：http://sjp.gaohongyu789.top

[S29] C：变参函数
来源：http://zon.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jiu.sxryk.cn

[S30] C：头文件保护
来源：http://ndu.shzxlz.cn

#ifndef X_H
来源：http://ins.tanke756.top

#define X_H
来源：http://mzg.shangyingyoupin.top

#endif
来源：http://mnh.fengsongda.top

[S31] C++：Hello World
来源：http://kzh.bjfxy.top

#include <iostream>
来源：http://vxc.vehdjk.com

int main() { std::cout << "Hello\n"; }
来源：http://qtq.ppjwa.cn

[S32] C++：字符串
来源：http://bce.vqdsnc.cn

std::string s = "hi";  s += "!";
来源：http://uux.jinyuanbaomall.cn

[S33] C++：vector 增删
来源：http://jzv.hysaishi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ltm.pycfn.com

[S34] C++：遍历 vector
来源：http://arl.chenzaomai.com

for (auto &x : v) { std::cout << x; }
来源：http://wdg.zycfv.cn

[S35] C++：map
来源：http://qpu.ydzc1.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wbk.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://xmw.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ivd.nanxuanxn.top

[S37] C++：set
来源：http://lwo.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dat.hesvh.cn

[S38] C++：排序
来源：http://pgu.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://uzv.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://ppc.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://got.cucudq.cn

[S40] C++：查找元素
来源：http://kal.chenlongwang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mty.cashguo.top

[S41] C++：类与构造函数
来源：http://eql.bjfxy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zbj.zhijiandao.cn

[S42] C++：继承与虚函数
来源：http://qhn.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://ole.zhijiandao.cn

[S43] C++：智能指针
来源：http://ofr.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://nig.gogol.net.cn

[S44] C++：引用传参
来源：http://piw.jinqigfzy.top

void inc(int &x) { ++x; }
来源：http://zhr.nwbrower.top

[S45] C++：lambda
来源：http://xlb.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://uet.meibo888.top

[S46] C++：函数模板
来源：http://gtu.hywenlv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ndt.hnxiangtu.top

[S47] C++：结构化绑定遍历
来源：http://bez.jlsjyb.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eax.tian-w.cn

[S48] C++：逐行读文件
来源：http://tpm.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://xth.vehdjk.com

while (std::getline(in, line)) { }
来源：http://wxc.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://zgs.gaohongyu789.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ugr.ctjpmb.com

[S50] C++：格式化数字
来源：http://vtw.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pnn.jiagoushi.top

[S51] C++：显式类型转换
来源：http://srw.yanxiufei.cn

static_cast<double>(a) / b
来源：http://krc.havefunace.top

[S52] C++：const 与 noexcept
来源：http://tuy.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://aio.cucudq.cn

[S53] C++：移动语义
来源：http://koi.gogol.net.cn

std::vector<int> w = std::move(v);
来源：http://kil.xingfuxueyuan.xyz

[S54] C++：异常处理
来源：http://yag.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sdf.uphjek.com

[S55] C++：结构化绑定
来源：http://abi.shuidangran.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rzw.yuxming.cn

[S56] C++：optional
来源：http://oil.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mgs.fehbvm.com

[S57] C++：编译期常量
来源：http://qfr.yuxming.cn

constexpr int N = 10;
来源：http://kki.cucudq.cn

[S58] C++：命名空间
来源：http://fui.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://xvt.epnwcf.com

[S59] C++：静态断言
来源：http://jdh.jiagoushi.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zth.gotoacloud.top

[S60] C++：遍历并删除元素
来源：http://gru.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fyf.jinghuilouyu.cn

================================================================================
来源：http://zfn.quarkkingdee.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qtw.ybcxt.top

================================================================================
来源：http://prc.epnwcf.com

[T01] Kotlin：Hello World
来源：http://dms.xuetiantiany.cn

println("Hello")
来源：http://bxl.jqgufenzy.top

[T02] Kotlin：变量
来源：http://tig.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ewr.fengsongda.top

[T03] Kotlin：字符串模板
来源：http://joc.wangdashe.top

"值: $b"
来源：http://lru.zhaomingkeji.xyz

[T04] Kotlin：空安全
来源：http://dlq.yj202588.top

val n: String? = null;  n?.length
来源：http://fgl.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://clr.wangdashe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nrd.wangdashe.top

[T06] Kotlin：集合映射
来源：http://xyx.52xcode.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tij.andypj.xyz

[T07] Kotlin：集合过滤
来源：http://fri.vqdsnc.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jdt.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://mij.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://dps.bjfxy.top


<!-- 参考信息 -->