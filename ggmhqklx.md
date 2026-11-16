代发 wailian999

readonly PI=3.14
来源：http://pss.gotoacloud.top

[R04] 位置参数
来源：http://izj.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://snl.tian-w.cn

[R05] 参数默认值
来源：http://esd.jianghu66.top

name="${1:-default}"
来源：http://ett.tanke756.top

[R06] 判断命令是否存在
来源：http://jxa.yvedp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nbx.hnxiangtu.top

[R07] if 判断文件
来源：http://ssx.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tzi.hammf.cn

[R08] 数值比较
来源：http://fzk.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://iuo.zhoulong.xyz

[R09] 字符串比较
来源：http://imb.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bew.hammf.cn

[R10] 正则匹配
来源：http://osc.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hvi.zhengqikj.top

[R11] case 多分支
来源：http://vwx.andypj.xyz

case "$1" in
来源：http://lni.zhiwuduotai.top

start) echo "启动" ;;
来源：http://ssd.9152youxi.cn

stop)  echo "停止" ;;
来源：http://sek.shuidangran.top

*)     echo "未知命令" ;;
来源：http://chm.ivvv.top

esac
来源：http://wjw.quarkkingdee.top

[R12] for 遍历文件
来源：http://jhv.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://tmd.ctjpmb.com

[R13] for 计数循环
来源：http://wos.ppjwa.cn

for i in {1..10}; do echo "$i"; done
来源：http://nav.cdnleiting.top

[R14] C 风格 for
来源：http://mst.c1oappe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://edf.hongshengwenyu.top

[R15] while 逐行读文件
来源：http://gsd.zhongyouzk.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://phi.zdbjq.cn

[R16] until 等待条件
来源：http://lmf.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://swg.9152youxi.cn

[R17] 数组定义与取值
来源：http://tyb.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://fcw.316326.xyz

[R18] 遍历数组
来源：http://bmu.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uqt.sjlbkw.cn

[R19] 数组长度
来源：http://mnu.fengsongda.top

echo "${#arr[@]}"
来源：http://ban.yj202588.top

[R20] 关联数组（字典）
来源：http://oag.cdnleiting.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qri.hysaishi.cn

[R21] 字符串长度
来源：http://vge.yj20258.top

echo "${#s}"
来源：http://xwh.hnqzz.top

[R22] 截取子串
来源：http://qfc.yongpay.top

echo "${s:0:5}"
来源：http://yfa.tanke756.top

[R23] 字符串替换
来源：http://bjj.bjfxy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://itj.c1oappe.top

[R24] 大小写转换
来源：http://shu.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://gnp.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://zal.jinqigfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xtm.redwolf501.top

[R26] 命令替换
来源：http://dgi.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://fov.shanyushiyangkeji.top

[R27] 算术展开
来源：http://dpj.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://rgh.shanyushiyangtech.top

[R28] 浮点运算
来源：http://glw.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://bzl.ydjk.org.cn

[R29] 定义函数
来源：http://inp.ivvv.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fvl.0kj1m.cn

[R30] 函数返回状态码
来源：http://ars.ivvv.top

f() { return 0; }; f || echo "失败了"
来源：http://aqr.ydzc1.top

[R31] 局部变量
来源：http://paj.9152youxi.cn

f() { local x=1; echo "$x"; }
来源：http://pjw.yvedp.cn

[R32] 参数个数校验
来源：http://jvx.jinyuanbaomall.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ymj.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://ykm.jqgfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gjl.jiagoushi.top

[R34] 退出时清理
来源：http://vit.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://mhg.andypj.xyz

[R35] 后台执行并等待
来源：http://joy.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dvj.smart0.xyz

[R36] 并发执行多个任务
来源：http://wie.nanxinkj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bxs.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://suj.hywenlv.cn

files=$(ls -1)
来源：http://hgo.cucudq.cn

[R38] 管道串联
来源：http://acz.shanyushiyangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://gyl.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://jsq.redwolf501.top

cmd > out.log 2>&1
来源：http://wpi.jinqigfzy.top

[R40] 追加写日志
来源：http://eaz.fengsongda.top

echo "log" >> out.log
来源：http://pzu.zhiwuduotai.top

[R41] 丢弃输出
来源：http://jgb.yfazqb.com

cmd >/dev/null 2>&1
来源：http://pon.uphjek.com

[R42] 输入重定向
来源：http://jmz.ivvv.top

wc -l < a.txt
来源：http://elp.tian-w.cn

[R43] 按名字查找文件
来源：http://eys.pengpengdd.cyou

find . -name "*.log" -type f
来源：http://ube.bjfxy.top

[R44] 按修改时间查找
来源：http://hgm.sweek.top

find . -mtime -7 -type f
来源：http://wym.chenzaomai.com

[R45] 批量删除
来源：http://foc.shuidangran.top

find . -name "*.tmp" -delete
来源：http://lnp.xuanzx.com

[R46] 递归替换文件内容
来源：http://iso.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qvw.zhongyouzk.top

[R47] sed 单行替换
来源：http://tvt.daxiang520.top

sed -i 's/foo/bar/g' a.txt
来源：http://drp.hnqzz.top

[R48] awk 取指定列
来源：http://dtf.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://dtb.zhixingplan.top

[R49] awk 带条件
来源：http://ice.yj202588.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bio.epnwcf.com

[R50] awk 求和
来源：http://otp.c1oappe.top

awk '{s += $2} END {print s}' a.txt
来源：http://ujz.snrcjt.cn

[R51] 排序去重取前几
来源：http://yit.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://iuk.gaohongyu789.top

[R52] 统计行数
来源：http://dmx.nwbrower.top

wc -l a.txt
来源：http://fap.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://ykj.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://acl.yongpay.top

[R54] 比较两个文件
来源：http://ymm.guannengcc.top

diff a.txt b.txt
来源：http://omx.jlsjyb.cn

[R55] 压缩与解压
来源：http://ggi.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ceg.guannengcc.top

[R56] 远程拷贝
来源：http://nkk.yangfankeji.com

scp file user@host:/path/
来源：http://fay.ydjk.org.cn

[R57] 远程执行命令
来源：http://nyd.shanyushiyangtech.top

ssh user@host 'uptime'
来源：http://bls.ivvv.top

[R58] 下载文件
来源：http://mfu.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zbf.52xcode.cn

[R59] 发 POST JSON
来源：http://omw.epnwcf.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gvj.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://bns.fzhhl.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wdb.fzhhl.top

[R61] 磁盘占用
来源：http://gyo.cucudq.cn

df -h;  du -sh *
来源：http://mrl.jyoumei.cn

[R62] 找最占空间的文件
来源：http://hbr.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://dbr.ybcxt.top

[R63] 内存与进程
来源：http://lol.sufxvd.cn

free -h;  ps aux | grep nginx
来源：http://awv.jyoumei.cn

[R64] 结束进程
来源：http://tyy.xuanzx.com

kill -9 $(pgrep -f app.py)
来源：http://kyt.chenzaomai.com

[R65] 查看端口占用
来源：http://cbf.redwolf501.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vji.vqdsnc.cn

[R66] 定时任务
来源：http://auj.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://buo.yuanzhike.top

[R67] 生成随机十六进制串
来源：http://xnm.zycfv.cn

openssl rand -hex 16
来源：http://orq.sjlbkw.cn

[R68] 计算文件校验值
来源：http://jwq.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://ltn.wangdashe.top

[R69] 生成随机密码
来源：http://rql.haohaochexian.top

head -c 16 /dev/urandom | base64
来源：http://rhv.hywenlv.cn

[R70] 时间戳与互转
来源：http://hou.daxiang520.top

date +%s;  date -d @1700000000
来源：http://eff.feifeiyinyue.top

[R71] 日期格式化
来源：http://nyh.jinqigfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://aya.jinqigfzy.top

[R72] 等待端口就绪
来源：http://rqz.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gzf.zhongyouzk.top

[R73] 分割大日志
来源：http://wna.yanxiufei.cn

split -l 1000 big.log part_
来源：http://gpx.tianlin.xyz

[R74] 批量重命名
来源：http://zpr.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pcf.zhongyouzk.top

[R75] 导出环境变量
来源：http://oyi.jinqigufen.top

export PATH="$HOME/bin:$PATH"
来源：http://rhk.aibaodan.cn

[R76] 使用临时文件
来源：http://fem.sufxvd.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pbh.zdqjudy.top

[R77] 读取用户输入
来源：http://xne.ivvv.top

read -rp "请输入: " ans
来源：http://lby.jqgfzy.top

[R78] 交互式菜单
来源：http://aaa.redwolf501.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yaj.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://wdy.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bkt.birdmap.top

[R80] 查看脚本执行耗时
来源：http://fdi.ivvv.top

time ./run.sh
来源：http://cit.daria6918.cn

================================================================================
来源：http://wkh.ehwqpu.com

S. C / C++ 专题
来源：http://pau.pengpengdd.cyou

================================================================================
来源：http://bom.yanxiufei.cn

[S01] C：Hello World
来源：http://tem.jinyuanbaomall.cn

#include <stdio.h>
来源：http://box.wangshuangyany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fal.xinyue.icu

[S02] C：变量与格式化输出
来源：http://gxw.tanke756.top

int a = 10; printf("%d\n", a);
来源：http://rvb.gaohongyu789.top

[S03] C：读入整数
来源：http://yym.yueranfly.top

int x; scanf("%d", &x);
来源：http://qsu.hnxiangtu.top

[S04] C：字符串复制
来源：http://xxr.ivvv.top

char dst[32]; strcpy(dst, "hi");
来源：http://edt.ydjk.org.cn

[S05] C：字符串长度
来源：http://jpu.kuanghao11.cn

strlen(s)
来源：http://xvk.yongpay.top

[S06] C：字符串比较
来源：http://ejg.mhx1999.top

strcmp(a, b) == 0
来源：http://tjr.cheryme.top

[S07] C：数组遍历求和
来源：http://yvn.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iaf.xingfuxueyuan.xyz

[S08] C：动态内存分配与释放
来源：http://wcb.jyoumei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nhy.wangshuangyany.cn

[S09] C：结构体定义与初始化
来源：http://wea.yuanzhike.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wni.epnwcf.com

[S10] C：指针与解引用
来源：http://bbm.hesvh.cn

int *p = &a;  *p = 5;
来源：http://bqc.birdmap.top

[S11] C：逐行读文件
来源：http://sry.jianghu66.top

FILE *f = fopen("a.txt", "r");
来源：http://nag.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://spg.zhijiandao.cn

fclose(f);
来源：http://ceb.jianghu66.top

[S12] C：写文件
来源：http://hhn.dashuyun.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zrj.aibaodan.cn

[S13] C：宏定义
来源：http://mqo.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bdg.daxiang520.top

[S14] C：枚举
来源：http://kbd.cqqwz.cn

enum Color { RED, GREEN, BLUE };
来源：http://fue.ppjwa.cn

[S15] C：类型转换
来源：http://wyc.xziqi.cn

(double) a / b
来源：http://okl.hysaishi.cn

[S16] C：位操作置位
来源：http://dka.shuidangran.top

x |= (1 << 3);
来源：http://qpy.sweek.top

[S17] C：安全拼接字符串
来源：http://hwf.svipenyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://khw.yangfankeji.com

[S18] C：命令行参数
来源：http://vbq.jianghu66.top

int main(int argc, char **argv)
来源：http://ftd.zhongyouzk.top

[S19] C：快速排序
来源：http://not.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://ira.0kj1m.cn

[S20] C：二分查找
来源：http://dmp.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ahn.yanxiufei.cn

[S21] C：字符类别判断
来源：http://xje.jinqigfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yzk.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://wuh.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yyi.jinyuanbaomall.cn

[S23] C：随机数
来源：http://sdd.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://mkq.xziqi.cn

[S24] C：获取本地时间
来源：http://nji.shuidangran.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://krr.ybcxt.top

[S25] C：内存拷贝
来源：http://xqu.zdbjq.cn

memcpy(dst, src, n);
来源：http://ywv.jinqigfzy.top

[S26] C：内存清零
来源：http://oai.birdmap.top

memset(a, 0, sizeof a);
来源：http://utj.dashuyun.cn

[S27] C：定义常量
来源：http://xbp.pengpengdd.cyou

const double PI = 3.14159;
来源：http://rlr.yj202588.top

[S28] C：静态变量
来源：http://tao.ybcxt.top

static int counter = 0;
来源：http://mfr.yanxiufei.cn

[S29] C：变参函数
来源：http://hge.zhiwuduotai.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tzu.hfpthk.cn

[S30] C：头文件保护
来源：http://vjk.hfpthk.cn

#ifndef X_H
来源：http://xbk.zdqjudy.top

#define X_H
来源：http://gnh.c1oappe.top

#endif
来源：http://nxf.havefunace.top

[S31] C++：Hello World
来源：http://rve.guowangkeji.top

#include <iostream>
来源：http://zrr.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://haf.haohaochexian.top

[S32] C++：字符串
来源：http://zwr.zhongyouzk.top

std::string s = "hi";  s += "!";
来源：http://nyp.aibaodan.cn

[S33] C++：vector 增删
来源：http://mlb.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mbf.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://udn.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://bse.cashguo.top

[S35] C++：map
来源：http://hax.daxiang520.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mpg.zhixingplan.top

[S36] C++：unordered_map
来源：http://pex.wangshuangyany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://afn.ppjwa.cn

[S37] C++：set
来源：http://krr.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qzb.quarkkingdee.top

[S38] C++：排序
来源：http://cag.xylfe.cn

std::sort(v.begin(), v.end());
来源：http://kkb.daria6918.cn

[S39] C++：自定义比较器排序
来源：http://slh.xinyue.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aqi.ydjk.org.cn

[S40] C++：查找元素
来源：http://gsx.yangfankeji.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://get.316326.xyz

[S41] C++：类与构造函数
来源：http://peh.hfpthk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aqz.iojbl.cn

[S42] C++：继承与虚函数
来源：http://zxb.hysaishi.cn

class B : public Base { public: void f() override {} };
来源：http://wmc.gogol.net.cn

[S43] C++：智能指针
来源：http://ofi.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://ant.tarul.cn

[S44] C++：引用传参
来源：http://fdz.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://rnw.snrcjt.cn

[S45] C++：lambda
来源：http://und.c1oappe.top

auto add = [](int a, int b) { return a + b; };
来源：http://pho.pycfn.com

[S46] C++：函数模板
来源：http://sti.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fym.chenzaomai.com

[S47] C++：结构化绑定遍历
来源：http://dtk.xingfuxueyuan.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://imi.epnwcf.com

[S48] C++：逐行读文件
来源：http://ktv.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://dyn.sxryk.cn

while (std::getline(in, line)) { }
来源：http://uea.yj20258.top

[S49] C++：写文件
来源：http://gwr.sxryk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://giz.jyoumei.cn

[S50] C++：格式化数字
来源：http://vex.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nzd.sysykeji.top

[S51] C++：显式类型转换
来源：http://ixm.hywenlv.cn

static_cast<double>(a) / b
来源：http://rop.vqdsnc.cn

[S52] C++：const 与 noexcept
来源：http://xbm.jyoumei.cn

int size() const noexcept { return n_; }
来源：http://sgq.sufxvd.cn

[S53] C++：移动语义
来源：http://gpg.daria6918.cn

std::vector<int> w = std::move(v);
来源：http://jgs.jyoumei.cn

[S54] C++：异常处理
来源：http://ror.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oba.sweek.top

[S55] C++：结构化绑定
来源：http://ypm.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nqt.hammf.cn

[S56] C++：optional
来源：http://cnf.pengpengdd.cyou

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cjx.hongshengwenyu.top

[S57] C++：编译期常量
来源：http://zjn.hfpthk.cn

constexpr int N = 10;
来源：http://rbp.cqqwz.cn

[S58] C++：命名空间
来源：http://hbq.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://jvi.ybcxt.top

[S59] C++：静态断言
来源：http://xpe.hesvh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aag.ybcxt.top

[S60] C++：遍历并删除元素
来源：http://qmg.yueranfly.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yig.jianghu66.top

================================================================================
来源：http://ufq.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fog.vqdsnc.cn

================================================================================
来源：http://mcu.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://xbk.yj20258888.top

println("Hello")
来源：http://wye.tian-w.cn

[T02] Kotlin：变量
来源：http://ham.guowangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ydk.aizwys.cn

[T03] Kotlin：字符串模板
来源：http://qfb.xinyue.icu

"值: $b"
来源：http://jaq.yonumen.top

[T04] Kotlin：空安全
来源：http://wtm.hysaishi.cn

val n: String? = null;  n?.length
来源：http://dee.iojbl.cn


<!-- 参考信息 -->