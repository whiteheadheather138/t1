代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mas.zhongyouzk.top

[R08] 数值比较
来源：http://laz.svipenyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hge.bjfxy.top

[R09] 字符串比较
来源：http://qfu.9152youxi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zuq.zhaomingkeji.xyz

[R10] 正则匹配
来源：http://tmi.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jvp.vehdjk.com

[R11] case 多分支
来源：http://tfv.yj202588.top

case "$1" in
来源：http://ixq.gaohongyu789.top

start) echo "启动" ;;
来源：http://ena.havefunace.top

stop)  echo "停止" ;;
来源：http://aeq.hywenlv.cn

*)     echo "未知命令" ;;
来源：http://xha.xziqi.cn

esac
来源：http://jfe.jinghuilouyu.cn

[R12] for 遍历文件
来源：http://wif.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://sir.uphjek.com

[R13] for 计数循环
来源：http://sfn.vehdjk.com

for i in {1..10}; do echo "$i"; done
来源：http://nxz.sufxvd.cn

[R14] C 风格 for
来源：http://jbi.svipenyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://raq.ehwqpu.com

[R15] while 逐行读文件
来源：http://wmv.havefunace.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xku.9152youxi.cn

[R16] until 等待条件
来源：http://wvj.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kny.birdmap.top

[R17] 数组定义与取值
来源：http://pfu.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://voa.guannengcc.top

[R18] 遍历数组
来源：http://rbm.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ilg.zhiwuduotai.top

[R19] 数组长度
来源：http://jsz.jiagoushi.top

echo "${#arr[@]}"
来源：http://gvd.hywenlv.cn

[R20] 关联数组（字典）
来源：http://soc.shangyingyoupin.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bla.sweek.top

[R21] 字符串长度
来源：http://wad.daxiang520.top

echo "${#s}"
来源：http://bqn.ydjk.org.cn

[R22] 截取子串
来源：http://tkv.zhijiandao.cn

echo "${s:0:5}"
来源：http://jhk.jyoumei.cn

[R23] 字符串替换
来源：http://xrn.sysykeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hlh.vehdjk.com

[R24] 大小写转换
来源：http://sdr.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://wni.nwbrower.top

[R25] 去后缀 / 去前缀
来源：http://tjx.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://rcl.chenlongwang.top

[R26] 命令替换
来源：http://ukc.jqgufenzy.top

now=$(date +%F); echo "$now"
来源：http://shx.jinqigufen.top

[R27] 算术展开
来源：http://sxw.feifeiyinyue.top

echo $((1 + 2 * 3))
来源：http://btl.sxryk.cn

[R28] 浮点运算
来源：http://zan.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://zna.tian-w.cn

[R29] 定义函数
来源：http://raw.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qgx.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://mzw.tianlin.xyz

f() { return 0; }; f || echo "失败了"
来源：http://ynt.zhijiandao.cn

[R31] 局部变量
来源：http://brs.andypj.xyz

f() { local x=1; echo "$x"; }
来源：http://jhf.tian-w.cn

[R32] 参数个数校验
来源：http://ibs.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://upf.yongpay.top

[R33] 捕获错误并提示行号
来源：http://meo.xziqi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qwg.shanyushiyangkeji.top

[R34] 退出时清理
来源：http://dju.shanyushiyangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://php.zdbjq.cn

[R35] 后台执行并等待
来源：http://hcv.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://iyc.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://hfg.cheryme.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gcm.redwolf501.top

[R37] 把输出赋给变量
来源：http://nxn.birdmap.top

files=$(ls -1)
来源：http://ogt.sufxvd.cn

[R38] 管道串联
来源：http://dfj.chenlongwang.top

cat a.txt | grep -i error | wc -l
来源：http://wgm.jinyuanbaomall.cn

[R39] 重定向标准输出与错误
来源：http://ivd.vqdsnc.cn

cmd > out.log 2>&1
来源：http://crz.fanxiaobao.xyz

[R40] 追加写日志
来源：http://tuy.yanxiufei.cn

echo "log" >> out.log
来源：http://rxd.jiagoushi.top

[R41] 丢弃输出
来源：http://lmq.cucudq.cn

cmd >/dev/null 2>&1
来源：http://lnu.jiagoushi.top

[R42] 输入重定向
来源：http://umd.ctjpmb.com

wc -l < a.txt
来源：http://jyl.hnxiangtu.top

[R43] 按名字查找文件
来源：http://dca.daxiang520.top

find . -name "*.log" -type f
来源：http://vre.havefunace.top

[R44] 按修改时间查找
来源：http://jln.gogol.net.cn

find . -mtime -7 -type f
来源：http://wye.fehbvm.com

[R45] 批量删除
来源：http://odf.jiagoushi.top

find . -name "*.tmp" -delete
来源：http://vna.svipenyu.cn

[R46] 递归替换文件内容
来源：http://ysb.iojbl.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sat.zhaomingkeji.xyz

[R47] sed 单行替换
来源：http://beb.wangdashe.top

sed -i 's/foo/bar/g' a.txt
来源：http://upk.hywenlv.cn

[R48] awk 取指定列
来源：http://sbx.xuanzx.com

awk '{print $1, $3}' a.txt
来源：http://jus.ydzc1.top

[R49] awk 带条件
来源：http://stw.cdnleiting.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gcn.daria6918.cn

[R50] awk 求和
来源：http://dkx.gotoacloud.top

awk '{s += $2} END {print s}' a.txt
来源：http://llg.haohaochexian.top

[R51] 排序去重取前几
来源：http://dyn.mhx1999.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pcs.gotoacloud.top

[R52] 统计行数
来源：http://qlj.pycfn.com

wc -l a.txt
来源：http://vih.fengsongda.top

[R53] 查看文件头与实时尾
来源：http://srs.daria6918.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pjx.gotoacloud.top

[R54] 比较两个文件
来源：http://ytj.yonumen.top

diff a.txt b.txt
来源：http://kbo.shanyushiyangtech.top

[R55] 压缩与解压
来源：http://okt.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wci.hfpthk.cn

[R56] 远程拷贝
来源：http://zyo.sysykeji.top

scp file user@host:/path/
来源：http://xif.pycfn.com

[R57] 远程执行命令
来源：http://jto.guannengcc.top

ssh user@host 'uptime'
来源：http://zzu.ydjk.org.cn

[R58] 下载文件
来源：http://afa.tianlin.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eun.yonumen.top

[R59] 发 POST JSON
来源：http://hjh.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dil.guowangkeji.top

[R60] 只看 HTTP 状态码
来源：http://bzd.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bsg.yangfankeji.com

[R61] 磁盘占用
来源：http://dvi.gaohongyu789.top

df -h;  du -sh *
来源：http://cae.tianlin.xyz

[R62] 找最占空间的文件
来源：http://epi.dianchejie.cn

du -ah . | sort -rh | head -10
来源：http://fup.xuanzx.com

[R63] 内存与进程
来源：http://nyn.ctjpmb.com

free -h;  ps aux | grep nginx
来源：http://okd.xinyue.icu

[R64] 结束进程
来源：http://aqd.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://hry.ybcxt.top

[R65] 查看端口占用
来源：http://mxs.52xcode.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vof.aizwys.cn

[R66] 定时任务
来源：http://sdp.daria6918.cn

crontab -e;  crontab -l
来源：http://vgq.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://xvb.jqgufenzy.top

openssl rand -hex 16
来源：http://xle.yj202588.top

[R68] 计算文件校验值
来源：http://zip.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iba.yuxming.cn

[R69] 生成随机密码
来源：http://vid.xinyue.icu

head -c 16 /dev/urandom | base64
来源：http://bbs.iojbl.cn

[R70] 时间戳与互转
来源：http://efd.daxiang520.top

date +%s;  date -d @1700000000
来源：http://tyl.gzhubu.top

[R71] 日期格式化
来源：http://hcc.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ayv.sufxvd.cn

[R72] 等待端口就绪
来源：http://pmd.sjlbkw.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nzl.guannengcc.top

[R73] 分割大日志
来源：http://rvg.ctjpmb.com

split -l 1000 big.log part_
来源：http://qzx.zhijiandao.cn

[R74] 批量重命名
来源：http://cwj.dashuyun.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xxg.chenlongwang.top

[R75] 导出环境变量
来源：http://avf.xingfuxueyuan.xyz

export PATH="$HOME/bin:$PATH"
来源：http://acx.0kj1m.cn

[R76] 使用临时文件
来源：http://pju.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kad.snrcjt.cn

[R77] 读取用户输入
来源：http://tst.fehbvm.com

read -rp "请输入: " ans
来源：http://iqo.dianchejie.cn

[R78] 交互式菜单
来源：http://muk.316326.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://upx.zhaomingkeji.xyz

[R79] 解析命令行选项
来源：http://tyf.yonumen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jub.zycfv.cn

[R80] 查看脚本执行耗时
来源：http://uig.guowangkeji.top

time ./run.sh
来源：http://rgu.dashuyun.cn

================================================================================
来源：http://kfb.hnxiangtu.top

S. C / C++ 专题
来源：http://ffc.jinqigfzy.top

================================================================================
来源：http://siv.zhengqikj.top

[S01] C：Hello World
来源：http://rce.snrcjt.cn

#include <stdio.h>
来源：http://hry.cucudq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gwf.zycfv.cn

[S02] C：变量与格式化输出
来源：http://eev.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://kdx.redwolf501.top

[S03] C：读入整数
来源：http://gwt.xziqi.cn

int x; scanf("%d", &x);
来源：http://clj.cucudq.cn

[S04] C：字符串复制
来源：http://apm.jqgufenzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://pno.andypj.xyz

[S05] C：字符串长度
来源：http://omq.aibaodan.cn

strlen(s)
来源：http://qdj.chenjidiqi.icu

[S06] C：字符串比较
来源：http://isz.aibaodan.cn

strcmp(a, b) == 0
来源：http://qsy.pycfn.com

[S07] C：数组遍历求和
来源：http://wcg.ehwqpu.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tdq.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://kgc.zdqjudy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rkf.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://fqv.sjlbkw.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iyz.birdmap.top

[S10] C：指针与解引用
来源：http://eyk.yuxming.cn

int *p = &a;  *p = 5;
来源：http://pou.epnwcf.com

[S11] C：逐行读文件
来源：http://vir.xylfe.cn

FILE *f = fopen("a.txt", "r");
来源：http://ihp.meibo888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wrb.xylfe.cn

fclose(f);
来源：http://faz.haohaochexian.top

[S12] C：写文件
来源：http://pbe.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://teh.pengpengdd.cyou

[S13] C：宏定义
来源：http://ama.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zzo.zhaomingkeji.xyz

[S14] C：枚举
来源：http://lvl.zdqjudy.top

enum Color { RED, GREEN, BLUE };
来源：http://nre.zhongyouzk.top

[S15] C：类型转换
来源：http://krb.xylfe.cn

(double) a / b
来源：http://nxc.yj20258888.top

[S16] C：位操作置位
来源：http://onk.dianchejie.cn

x |= (1 << 3);
来源：http://xgz.hysaishi.cn

[S17] C：安全拼接字符串
来源：http://pop.chenlongwang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sxw.yanxiufei.cn

[S18] C：命令行参数
来源：http://yoz.mhx1999.top

int main(int argc, char **argv)
来源：http://wto.daxiang520.top

[S19] C：快速排序
来源：http://cbi.ywan-chungtsiang.top

qsort(a, n, sizeof(int), cmp);
来源：http://eef.daria6918.cn

[S20] C：二分查找
来源：http://pmz.tarul.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zwm.ywan-chungtsiang.top

[S21] C：字符类别判断
来源：http://yat.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dso.sufxvd.cn

[S22] C：字符串转数字
来源：http://otd.aizwys.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tiq.snrcjt.cn

[S23] C：随机数
来源：http://hdm.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mhc.52xcode.cn

[S24] C：获取本地时间
来源：http://jom.zhiwuduotai.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ecm.jyoumei.cn

[S25] C：内存拷贝
来源：http://dgo.yonumen.top

memcpy(dst, src, n);
来源：http://hvp.shzxlz.cn

[S26] C：内存清零
来源：http://ipd.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://yye.yfazqb.com

[S27] C：定义常量
来源：http://jsa.hywenlv.cn

const double PI = 3.14159;
来源：http://rhk.haohaochexian.top

[S28] C：静态变量
来源：http://ofy.dashuyun.cn

static int counter = 0;
来源：http://ziz.snrcjt.cn

[S29] C：变参函数
来源：http://xgn.jqgfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://axv.shanyushiyangkeji.top

[S30] C：头文件保护
来源：http://muc.fktsv.cn

#ifndef X_H
来源：http://stk.xingfuxueyuan.xyz

#define X_H
来源：http://rmh.dashuyun.cn

#endif
来源：http://whe.ydzc1.top

[S31] C++：Hello World
来源：http://eft.tarul.cn

#include <iostream>
来源：http://myh.yuanzhike.top

int main() { std::cout << "Hello\n"; }
来源：http://wol.yanxiufei.cn

[S32] C++：字符串
来源：http://tor.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://uug.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://mzp.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aac.hnqzz.top

[S34] C++：遍历 vector
来源：http://cei.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://acv.dashuyun.cn

[S35] C++：map
来源：http://mqr.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hre.jyoumei.cn

[S36] C++：unordered_map
来源：http://ate.zhiwuduotai.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jwk.jianghu66.top

[S37] C++：set
来源：http://jqm.snrcjt.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://inp.vehdjk.com

[S38] C++：排序
来源：http://mmb.vehdjk.com

std::sort(v.begin(), v.end());
来源：http://nqm.ivvv.top

[S39] C++：自定义比较器排序
来源：http://wql.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aqm.dianchejie.cn

[S40] C++：查找元素
来源：http://sga.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://glv.yangfankeji.com

[S41] C++：类与构造函数
来源：http://zun.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rqr.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://sxq.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://txz.redwolf501.top

[S43] C++：智能指针
来源：http://hqq.hongshengwenyu.top

auto p = std::make_unique<int>(5);
来源：http://eof.xylfe.cn

[S44] C++：引用传参
来源：http://dbb.xinyue.icu

void inc(int &x) { ++x; }
来源：http://kuu.yongpay.top

[S45] C++：lambda
来源：http://mql.xuetiantiany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rrt.mhx1999.top

[S46] C++：函数模板
来源：http://mwb.svipenyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vty.yj202588.top

[S47] C++：结构化绑定遍历
来源：http://twf.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wqp.jyoumei.cn

[S48] C++：逐行读文件
来源：http://fno.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://mhj.vehdjk.com

while (std::getline(in, line)) { }
来源：http://lrj.meibo888.top

[S49] C++：写文件
来源：http://yqe.jiagoushi.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yas.zhengqikj.top

[S50] C++：格式化数字
来源：http://xlq.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://msb.bbcook.cn

[S51] C++：显式类型转换
来源：http://fde.zhoulong.xyz

static_cast<double>(a) / b
来源：http://gbr.yvedp.cn

[S52] C++：const 与 noexcept
来源：http://bsr.xziqi.cn

int size() const noexcept { return n_; }
来源：http://ezm.hnqzz.top

[S53] C++：移动语义
来源：http://amv.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://aja.hammf.cn

[S54] C++：异常处理
来源：http://bxy.tanke756.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yiq.cqqwz.cn

[S55] C++：结构化绑定
来源：http://wbw.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jwv.jinghuilouyu.cn

[S56] C++：optional
来源：http://gnj.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://npr.ctjpmb.com

[S57] C++：编译期常量
来源：http://cth.nanxuanxn.top

constexpr int N = 10;
来源：http://zts.dianchejie.cn

[S58] C++：命名空间
来源：http://cug.shangyingyoupin.top

namespace ns { int f() { return 1; } }
来源：http://omd.shangyingyoupin.top

[S59] C++：静态断言
来源：http://wad.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rmt.yj20258.top

[S60] C++：遍历并删除元素
来源：http://sdi.dianchejie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ruv.hnxiangtu.top

================================================================================
来源：http://kke.chenjidiqi.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nkh.jianghu66.top

================================================================================
来源：http://zrw.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://nwa.c1oappe.top

println("Hello")
来源：http://qoh.yonumen.top

[T02] Kotlin：变量
来源：http://ptg.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://azj.ywan-chungtsiang.top

[T03] Kotlin：字符串模板
来源：http://ljh.cqqwz.cn

"值: $b"
来源：http://rmi.yongpay.top

[T04] Kotlin：空安全
来源：http://hds.sufxvd.cn

val n: String? = null;  n?.length
来源：http://mgm.tanke756.top

[T05] Kotlin：when 表达式
来源：http://jfn.dashuyun.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wwb.chenjidiqi.icu

[T06] Kotlin：集合映射
来源：http://vub.meibo888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://htq.hcnkem.com

[T07] Kotlin：集合过滤
来源：http://bnz.feifeiyinyue.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jnq.uphjek.com

[T08] Kotlin：数据类
来源：http://cet.c1oappe.top

data class User(val name: String, val age: Int)
来源：http://rwx.wangdashe.top


<!-- 参考信息 -->