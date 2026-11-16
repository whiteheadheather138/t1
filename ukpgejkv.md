代发 wailian999

case "$1" in
来源：http://oqo.fengsongda.top

start) echo "启动" ;;
来源：http://mlj.dashuyun.cn

stop)  echo "停止" ;;
来源：http://uux.pycfn.com

*)     echo "未知命令" ;;
来源：http://gim.hongshengwenyu.top

esac
来源：http://ayh.jinyuanbaomall.cn

[R12] for 遍历文件
来源：http://lnf.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://cri.zycfv.cn

[R13] for 计数循环
来源：http://coo.dianchejie.cn

for i in {1..10}; do echo "$i"; done
来源：http://gcx.xuetiantiany.cn

[R14] C 风格 for
来源：http://vjt.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xjc.hnxiangtu.top

[R15] while 逐行读文件
来源：http://cav.tianlin.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cnr.snrcjt.cn

[R16] until 等待条件
来源：http://hal.chenlongwang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://omw.yj202588.top

[R17] 数组定义与取值
来源：http://sjh.fzhhl.top

arr=(a b c); echo "${arr[0]}"
来源：http://dtj.tianlin.xyz

[R18] 遍历数组
来源：http://ixo.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hdl.xuanzx.com

[R19] 数组长度
来源：http://xit.fehbvm.com

echo "${#arr[@]}"
来源：http://sme.redwolf501.top

[R20] 关联数组（字典）
来源：http://chn.yanxiufei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nll.xingfuxueyuan.xyz

[R21] 字符串长度
来源：http://scp.yueranfly.top

echo "${#s}"
来源：http://cqi.shanyushiyangtech.top

[R22] 截取子串
来源：http://vyi.andypj.xyz

echo "${s:0:5}"
来源：http://dpk.havefunace.top

[R23] 字符串替换
来源：http://isc.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xwc.yfazqb.com

[R24] 大小写转换
来源：http://jyk.nanxuanxn.top

echo "${s^^}"; echo "${s,,}"
来源：http://iqc.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://qzq.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://ipz.zhoulong.xyz

[R26] 命令替换
来源：http://kfb.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://int.hywenlv.cn

[R27] 算术展开
来源：http://gzp.yfazqb.com

echo $((1 + 2 * 3))
来源：http://vsz.jinqigufen.top

[R28] 浮点运算
来源：http://mcz.tarul.cn

echo "scale=2; 10/3" | bc
来源：http://vml.mhx1999.top

[R29] 定义函数
来源：http://urs.nwbrower.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xlh.zhengqikj.top

[R30] 函数返回状态码
来源：http://ewg.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://shl.dashuyun.cn

[R31] 局部变量
来源：http://fvo.xingfuxueyuan.xyz

f() { local x=1; echo "$x"; }
来源：http://bah.gzhubu.top

[R32] 参数个数校验
来源：http://idi.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vrv.havefunace.top

[R33] 捕获错误并提示行号
来源：http://wdl.havefunace.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zey.daria6918.cn

[R34] 退出时清理
来源：http://hgv.epnwcf.com

trap 'rm -f "$tmp"' EXIT
来源：http://tnr.nanxuanxn.top

[R35] 后台执行并等待
来源：http://kcq.aibaodan.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mvq.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://obp.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ooa.ybcxt.top

[R37] 把输出赋给变量
来源：http://bdl.svipenyu.cn

files=$(ls -1)
来源：http://orm.0kj1m.cn

[R38] 管道串联
来源：http://dog.gzhubu.top

cat a.txt | grep -i error | wc -l
来源：http://tyo.xingfuxueyuan.xyz

[R39] 重定向标准输出与错误
来源：http://pcd.fzhhl.top

cmd > out.log 2>&1
来源：http://bas.ywan-chungtsiang.top

[R40] 追加写日志
来源：http://bbr.xinyue.icu

echo "log" >> out.log
来源：http://oyz.jlsjyb.cn

[R41] 丢弃输出
来源：http://ocg.nwbrower.top

cmd >/dev/null 2>&1
来源：http://xwu.yj20258.top

[R42] 输入重定向
来源：http://lvo.yonumen.top

wc -l < a.txt
来源：http://amx.hysaishi.cn

[R43] 按名字查找文件
来源：http://sdx.snrcjt.cn

find . -name "*.log" -type f
来源：http://hqa.ivvv.top

[R44] 按修改时间查找
来源：http://gsy.nanxuanxn.top

find . -mtime -7 -type f
来源：http://odl.zhengqikj.top

[R45] 批量删除
来源：http://egm.ehwqpu.com

find . -name "*.tmp" -delete
来源：http://epg.52xcode.cn

[R46] 递归替换文件内容
来源：http://joz.hysaishi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ssx.jinghuilouyu.cn

[R47] sed 单行替换
来源：http://zrl.yj202588.top

sed -i 's/foo/bar/g' a.txt
来源：http://smu.aizwys.cn

[R48] awk 取指定列
来源：http://cdq.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://ngs.zhijiandao.cn

[R49] awk 带条件
来源：http://mkm.xinyue.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gov.fzhhl.top

[R50] awk 求和
来源：http://pkb.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://vbq.c1oappe.top

[R51] 排序去重取前几
来源：http://zcc.cheryme.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hbt.tianlin.xyz

[R52] 统计行数
来源：http://hbq.nwbrower.top

wc -l a.txt
来源：http://oau.cheryme.top

[R53] 查看文件头与实时尾
来源：http://frr.feifeiyinyue.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uhk.andypj.xyz

[R54] 比较两个文件
来源：http://rjl.guannengcc.top

diff a.txt b.txt
来源：http://rki.redwolf501.top

[R55] 压缩与解压
来源：http://jis.cheryme.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://csl.iojbl.cn

[R56] 远程拷贝
来源：http://bch.cheryme.top

scp file user@host:/path/
来源：http://yya.hnqzz.top

[R57] 远程执行命令
来源：http://guw.smart0.xyz

ssh user@host 'uptime'
来源：http://bpt.yfazqb.com

[R58] 下载文件
来源：http://qww.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://enw.yonumen.top

[R59] 发 POST JSON
来源：http://gtl.ppjwa.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ovq.jyoumei.cn

[R60] 只看 HTTP 状态码
来源：http://qbp.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://did.bbcook.cn

[R61] 磁盘占用
来源：http://daa.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://dba.guannengcc.top

[R62] 找最占空间的文件
来源：http://fac.yonumen.top

du -ah . | sort -rh | head -10
来源：http://kpo.fehbvm.com

[R63] 内存与进程
来源：http://ams.zhijiandao.cn

free -h;  ps aux | grep nginx
来源：http://koc.hnxiangtu.top

[R64] 结束进程
来源：http://jou.cqqwz.cn

kill -9 $(pgrep -f app.py)
来源：http://uyc.ivvv.top

[R65] 查看端口占用
来源：http://igp.jiagoushi.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jnu.tianlin.xyz

[R66] 定时任务
来源：http://hmm.c1oappe.top

crontab -e;  crontab -l
来源：http://zwf.jiagoushi.top

[R67] 生成随机十六进制串
来源：http://qkx.feifeiyinyue.top

openssl rand -hex 16
来源：http://cqz.yueranfly.top

[R68] 计算文件校验值
来源：http://yqi.hcnkem.com

sha256sum a.txt;  md5sum a.txt
来源：http://bun.9152youxi.cn

[R69] 生成随机密码
来源：http://pxi.tanke756.top

head -c 16 /dev/urandom | base64
来源：http://jqh.shzxlz.cn

[R70] 时间戳与互转
来源：http://mbt.fanxiaobao.xyz

date +%s;  date -d @1700000000
来源：http://jng.xuanzx.com

[R71] 日期格式化
来源：http://ajx.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nnm.guowangkeji.top

[R72] 等待端口就绪
来源：http://xcv.havefunace.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mnb.meibo888.top

[R73] 分割大日志
来源：http://awt.jinqigfzy.top

split -l 1000 big.log part_
来源：http://yxr.wangshuangyany.cn

[R74] 批量重命名
来源：http://ifg.yuxming.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://coj.0kj1m.cn

[R75] 导出环境变量
来源：http://wqi.yangfankeji.com

export PATH="$HOME/bin:$PATH"
来源：http://aix.yongpay.top

[R76] 使用临时文件
来源：http://yxd.hysaishi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vdd.dianchejie.cn

[R77] 读取用户输入
来源：http://kst.fehbvm.com

read -rp "请输入: " ans
来源：http://ykh.yj202588.top

[R78] 交互式菜单
来源：http://mrw.jlsjyb.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pci.meibo888.top

[R79] 解析命令行选项
来源：http://jsm.aibaodan.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kqq.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://stf.vqdsnc.cn

time ./run.sh
来源：http://ggd.gaohongyu789.top

================================================================================
来源：http://ucv.316326.xyz

S. C / C++ 专题
来源：http://tvu.wangdashe.top

================================================================================
来源：http://dsy.zdqjudy.top

[S01] C：Hello World
来源：http://gip.fktsv.cn

#include <stdio.h>
来源：http://nxi.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nss.bbcook.cn

[S02] C：变量与格式化输出
来源：http://lnb.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://krr.zdqjudy.top

[S03] C：读入整数
来源：http://acr.havefunace.top

int x; scanf("%d", &x);
来源：http://tmg.chenjidiqi.icu

[S04] C：字符串复制
来源：http://van.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xvk.smart0.xyz

[S05] C：字符串长度
来源：http://gjh.jiagoushi.top

strlen(s)
来源：http://lzh.gotoacloud.top

[S06] C：字符串比较
来源：http://lcd.hcnkem.com

strcmp(a, b) == 0
来源：http://rqb.jlsjyb.cn

[S07] C：数组遍历求和
来源：http://fjr.jinqigfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wdf.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://kij.nanxinkj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iqo.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://jmt.redwolf501.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pba.mhx1999.top

[S10] C：指针与解引用
来源：http://zpd.zhixingplan.top

int *p = &a;  *p = 5;
来源：http://jtd.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://jsn.mhx1999.top

FILE *f = fopen("a.txt", "r");
来源：http://gli.xuetiantiany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sfa.bjfxy.top

fclose(f);
来源：http://ymn.ctjpmb.com

[S12] C：写文件
来源：http://jes.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://onp.redwolf501.top

[S13] C：宏定义
来源：http://bht.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ycq.jlsjyb.cn

[S14] C：枚举
来源：http://idw.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://tbs.jqgfzy.top

[S15] C：类型转换
来源：http://qvo.chenjidiqi.icu

(double) a / b
来源：http://fnh.vehdjk.com

[S16] C：位操作置位
来源：http://ebq.yuanzhike.top

x |= (1 << 3);
来源：http://fpt.yuxming.cn

[S17] C：安全拼接字符串
来源：http://nrw.tianlin.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wra.fzhhl.top

[S18] C：命令行参数
来源：http://jvt.sufxvd.cn

int main(int argc, char **argv)
来源：http://fuc.fengsongda.top

[S19] C：快速排序
来源：http://nmn.cqqwz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qlw.tianlin.xyz

[S20] C：二分查找
来源：http://zgw.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mcz.zycfv.cn

[S21] C：字符类别判断
来源：http://iyu.jianghu66.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xuu.zycfv.cn

[S22] C：字符串转数字
来源：http://woi.fengsongda.top

atoi("42");  strtod("3.14", NULL);
来源：http://aoo.yuxming.cn

[S23] C：随机数
来源：http://oew.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pwz.andypj.xyz

[S24] C：获取本地时间
来源：http://jii.sysykeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oxh.zdbjq.cn

[S25] C：内存拷贝
来源：http://dpr.vehdjk.com

memcpy(dst, src, n);
来源：http://nsm.fanxiaobao.xyz

[S26] C：内存清零
来源：http://uug.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://dze.hongshengwenyu.top

[S27] C：定义常量
来源：http://ygf.jianghu66.top

const double PI = 3.14159;
来源：http://dsg.xuetiantiany.cn

[S28] C：静态变量
来源：http://szo.nwbrower.top

static int counter = 0;
来源：http://svr.cucudq.cn

[S29] C：变参函数
来源：http://yea.cucudq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tdn.guannengcc.top

[S30] C：头文件保护
来源：http://hek.uphjek.com

#ifndef X_H
来源：http://izi.wangshuangyany.cn

#define X_H
来源：http://wbn.vqdsnc.cn

#endif
来源：http://jcl.sjlbkw.cn

[S31] C++：Hello World
来源：http://nwf.jinqigufen.top

#include <iostream>
来源：http://pqc.hesvh.cn

int main() { std::cout << "Hello\n"; }
来源：http://eha.fktsv.cn

[S32] C++：字符串
来源：http://ige.vehdjk.com

std::string s = "hi";  s += "!";
来源：http://dwe.ydjk.org.cn

[S33] C++：vector 增删
来源：http://bwm.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cgo.pengpengdd.cyou

[S34] C++：遍历 vector
来源：http://ezy.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://unx.zhoulong.xyz

[S35] C++：map
来源：http://dor.yuanzhike.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fsc.wangshuangyany.cn

[S36] C++：unordered_map
来源：http://zdo.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://otn.sxryk.cn

[S37] C++：set
来源：http://rhb.hcnkem.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yid.hesvh.cn

[S38] C++：排序
来源：http://gcs.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://kid.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://ame.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://noz.pycfn.com

[S40] C++：查找元素
来源：http://rjl.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uxe.chenjidiqi.icu

[S41] C++：类与构造函数
来源：http://btx.haohaochexian.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gtj.bbcook.cn

[S42] C++：继承与虚函数
来源：http://jha.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://mkk.wangshuangyany.cn

[S43] C++：智能指针
来源：http://ukb.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://wll.yueranfly.top

[S44] C++：引用传参
来源：http://ifr.hongshengwenyu.top

void inc(int &x) { ++x; }
来源：http://foe.uphjek.com

[S45] C++：lambda
来源：http://ova.kuanghao11.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nbp.vqdsnc.cn

[S46] C++：函数模板
来源：http://rai.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ect.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://rvh.ivvv.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tdm.redwolf501.top

[S48] C++：逐行读文件
来源：http://uaw.sjlbkw.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ora.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://vii.meibo888.top

[S49] C++：写文件
来源：http://ljm.sjlbkw.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rwp.bjfxy.top

[S50] C++：格式化数字
来源：http://fju.guannengcc.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vxn.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://yyu.wangshuangyany.cn

static_cast<double>(a) / b
来源：http://hfb.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://jqe.yangfankeji.com

int size() const noexcept { return n_; }
来源：http://qxr.meibo888.top

[S53] C++：移动语义
来源：http://kml.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://mif.wangshuangyany.cn

[S54] C++：异常处理
来源：http://mvs.jinghuilouyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qre.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://zvp.shuidangran.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qbv.aibaodan.cn

[S56] C++：optional
来源：http://oou.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nvr.yj20258.top

[S57] C++：编译期常量
来源：http://fnm.jyoumei.cn

constexpr int N = 10;
来源：http://fqn.jqgufenzy.top

[S58] C++：命名空间
来源：http://muj.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://spw.chenjidiqi.icu

[S59] C++：静态断言
来源：http://mfe.kuanghao11.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zwm.yongpay.top

[S60] C++：遍历并删除元素
来源：http://nlm.tarul.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iwe.hnxiangtu.top

================================================================================
来源：http://evd.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fpk.shangyingyoupin.top

================================================================================
来源：http://lsq.ivvv.top

[T01] Kotlin：Hello World
来源：http://pwe.iojbl.cn

println("Hello")
来源：http://ukv.jlsjyb.cn

[T02] Kotlin：变量
来源：http://thz.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://usz.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://vcu.hcnkem.com

"值: $b"
来源：http://bfq.9152youxi.cn

[T04] Kotlin：空安全
来源：http://ljt.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://yjw.epnwcf.com

[T05] Kotlin：when 表达式
来源：http://yyp.fehbvm.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ash.haohaochexian.top

[T06] Kotlin：集合映射
来源：http://kxs.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qhz.nanxuanxn.top

[T07] Kotlin：集合过滤
来源：http://ygl.xingfuxueyuan.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://ned.birdmap.top

[T08] Kotlin：数据类
来源：http://pbe.zdqjudy.top

data class User(val name: String, val age: Int)
来源：http://tbx.zhiwuduotai.top

[T09] Kotlin：扩展函数
来源：http://ysw.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://ook.daria6918.cn

[T10] Kotlin：默认参数
来源：http://qxa.tianlin.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://cyi.pycfn.com

[T11] Kotlin：协程
来源：http://qlo.9152youxi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ptl.gogol.net.cn

[T12] Kotlin：解构声明
来源：http://hnd.yueranfly.top

val (a, b) = Pair(1, 2)
来源：http://iyi.cashguo.top


<!-- 参考信息 -->