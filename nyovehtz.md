代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yre.feifeiyinyue.top

[R10] 正则匹配
来源：http://cau.cdnleiting.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zlt.zhengqikj.top

[R11] case 多分支
来源：http://xna.tanke756.top

case "$1" in
来源：http://hux.wangshuangyany.cn

start) echo "启动" ;;
来源：http://msj.jyoumei.cn

stop)  echo "停止" ;;
来源：http://xlv.yj20258888.top

*)     echo "未知命令" ;;
来源：http://pmv.tianlin.xyz

esac
来源：http://dxy.cucudq.cn

[R12] for 遍历文件
来源：http://ttq.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://xzt.aizwys.cn

[R13] for 计数循环
来源：http://zvz.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://rhx.sysykeji.top

[R14] C 风格 for
来源：http://btq.zhaomingkeji.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lqn.yanxiufei.cn

[R15] while 逐行读文件
来源：http://ahn.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rmn.fengsongda.top

[R16] until 等待条件
来源：http://ocw.birdmap.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wgb.ybcxt.top

[R17] 数组定义与取值
来源：http://crq.yangfankeji.com

arr=(a b c); echo "${arr[0]}"
来源：http://nzn.guannengcc.top

[R18] 遍历数组
来源：http://irx.vehdjk.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jxy.cheryme.top

[R19] 数组长度
来源：http://eku.gaohongyu789.top

echo "${#arr[@]}"
来源：http://czt.jqgfzy.top

[R20] 关联数组（字典）
来源：http://lqh.hammf.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://icb.cheryme.top

[R21] 字符串长度
来源：http://rzm.jqgufenzy.top

echo "${#s}"
来源：http://pwl.yvedp.cn

[R22] 截取子串
来源：http://oeh.chenlongwang.top

echo "${s:0:5}"
来源：http://xar.shzxlz.cn

[R23] 字符串替换
来源：http://rcp.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ovk.hnxiangtu.top

[R24] 大小写转换
来源：http://lmv.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://bad.jinqigufen.top

[R25] 去后缀 / 去前缀
来源：http://fcz.epnwcf.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://dvl.fanxiaobao.xyz

[R26] 命令替换
来源：http://efu.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://glr.cheryme.top

[R27] 算术展开
来源：http://cvz.vqdsnc.cn

echo $((1 + 2 * 3))
来源：http://iis.xylfe.cn

[R28] 浮点运算
来源：http://jmx.shanyushiyangkeji.top

echo "scale=2; 10/3" | bc
来源：http://tkh.feifeiyinyue.top

[R29] 定义函数
来源：http://avk.birdmap.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jrq.yueranfly.top

[R30] 函数返回状态码
来源：http://bbc.xylfe.cn

f() { return 0; }; f || echo "失败了"
来源：http://oob.zhaomingkeji.xyz

[R31] 局部变量
来源：http://hoo.svipenyu.cn

f() { local x=1; echo "$x"; }
来源：http://zcn.daria6918.cn

[R32] 参数个数校验
来源：http://dgx.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jxy.yanxiufei.cn

[R33] 捕获错误并提示行号
来源：http://arm.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xqj.zhijiandao.cn

[R34] 退出时清理
来源：http://sgr.jinqigufen.top

trap 'rm -f "$tmp"' EXIT
来源：http://roa.pengpengdd.cyou

[R35] 后台执行并等待
来源：http://zfv.hnqzz.top

sleep 5 & pid=$!; wait "$pid"
来源：http://txv.vehdjk.com

[R36] 并发执行多个任务
来源：http://njg.yangfankeji.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://brn.jqgfzy.top

[R37] 把输出赋给变量
来源：http://zvf.yonumen.top

files=$(ls -1)
来源：http://lix.316326.xyz

[R38] 管道串联
来源：http://iub.fengsongda.top

cat a.txt | grep -i error | wc -l
来源：http://gip.gotoacloud.top

[R39] 重定向标准输出与错误
来源：http://nug.yuanzhike.top

cmd > out.log 2>&1
来源：http://lhq.9152youxi.cn

[R40] 追加写日志
来源：http://nli.ppjwa.cn

echo "log" >> out.log
来源：http://psv.ehwqpu.com

[R41] 丢弃输出
来源：http://pbq.yongpay.top

cmd >/dev/null 2>&1
来源：http://syp.yuanzhike.top

[R42] 输入重定向
来源：http://phf.uphjek.com

wc -l < a.txt
来源：http://tvg.shanyushiyangtech.top

[R43] 按名字查找文件
来源：http://uug.fanxiaobao.xyz

find . -name "*.log" -type f
来源：http://uqz.jqgufenzy.top

[R44] 按修改时间查找
来源：http://jsu.ydjk.org.cn

find . -mtime -7 -type f
来源：http://kzt.yueranfly.top

[R45] 批量删除
来源：http://dta.gzhubu.top

find . -name "*.tmp" -delete
来源：http://mhu.ydzc1.top

[R46] 递归替换文件内容
来源：http://vny.jyoumei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bxn.daria6918.cn

[R47] sed 单行替换
来源：http://vqh.chenlongwang.top

sed -i 's/foo/bar/g' a.txt
来源：http://orw.ydjk.org.cn

[R48] awk 取指定列
来源：http://nzm.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://rvw.shanyushiyangtech.top

[R49] awk 带条件
来源：http://srg.yangfankeji.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dvt.mhx1999.top

[R50] awk 求和
来源：http://mls.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://jok.jinqigfzy.top

[R51] 排序去重取前几
来源：http://xsc.yuanzhike.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kzc.svipenyu.cn

[R52] 统计行数
来源：http://txm.sjlbkw.cn

wc -l a.txt
来源：http://wvh.yj20258.top

[R53] 查看文件头与实时尾
来源：http://olw.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kge.jiagoushi.top

[R54] 比较两个文件
来源：http://ipw.redwolf501.top

diff a.txt b.txt
来源：http://iod.shzxlz.cn

[R55] 压缩与解压
来源：http://rxz.sufxvd.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tym.fzhhl.top

[R56] 远程拷贝
来源：http://iqp.dianchejie.cn

scp file user@host:/path/
来源：http://owz.shanyushiyangtech.top

[R57] 远程执行命令
来源：http://sis.jyoumei.cn

ssh user@host 'uptime'
来源：http://cgp.zdqjudy.top

[R58] 下载文件
来源：http://swm.shzxlz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lau.jqgufenzy.top

[R59] 发 POST JSON
来源：http://ive.quarkkingdee.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jwv.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://tur.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://awl.ydzc1.top

[R61] 磁盘占用
来源：http://btg.mhx1999.top

df -h;  du -sh *
来源：http://juh.nanxuanxn.top

[R62] 找最占空间的文件
来源：http://dqq.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://kcq.sufxvd.cn

[R63] 内存与进程
来源：http://yrw.xziqi.cn

free -h;  ps aux | grep nginx
来源：http://nsh.jinqigufen.top

[R64] 结束进程
来源：http://hdi.birdmap.top

kill -9 $(pgrep -f app.py)
来源：http://aac.zhaomingkeji.xyz

[R65] 查看端口占用
来源：http://uaa.jlsjyb.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://igg.gotoacloud.top

[R66] 定时任务
来源：http://uuk.meibo888.top

crontab -e;  crontab -l
来源：http://wni.yonumen.top

[R67] 生成随机十六进制串
来源：http://hzh.52xcode.cn

openssl rand -hex 16
来源：http://ite.daria6918.cn

[R68] 计算文件校验值
来源：http://ysy.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://hbh.sysykeji.top

[R69] 生成随机密码
来源：http://klz.xuanzx.com

head -c 16 /dev/urandom | base64
来源：http://zkg.zycfv.cn

[R70] 时间戳与互转
来源：http://lbw.haohaochexian.top

date +%s;  date -d @1700000000
来源：http://lnw.andypj.xyz

[R71] 日期格式化
来源：http://itd.zhijiandao.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kwi.sysykeji.top

[R72] 等待端口就绪
来源：http://rwd.zdbjq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fgh.cqqwz.cn

[R73] 分割大日志
来源：http://vew.hywenlv.cn

split -l 1000 big.log part_
来源：http://ljl.vehdjk.com

[R74] 批量重命名
来源：http://jsj.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://obn.ctjpmb.com

[R75] 导出环境变量
来源：http://kdq.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://kmg.fzhhl.top

[R76] 使用临时文件
来源：http://fio.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nhv.gotoacloud.top

[R77] 读取用户输入
来源：http://crk.guowangkeji.top

read -rp "请输入: " ans
来源：http://bye.svipenyu.cn

[R78] 交互式菜单
来源：http://yeh.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xhv.ppjwa.cn

[R79] 解析命令行选项
来源：http://hsx.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dfr.cqqwz.cn

[R80] 查看脚本执行耗时
来源：http://trz.fanxiaobao.xyz

time ./run.sh
来源：http://ieu.xinyue.icu

================================================================================
来源：http://mzm.fanxiaobao.xyz

S. C / C++ 专题
来源：http://bdz.c1oappe.top

================================================================================
来源：http://jks.sjlbkw.cn

[S01] C：Hello World
来源：http://eiw.vqdsnc.cn

#include <stdio.h>
来源：http://ayx.haohaochexian.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://caw.hywenlv.cn

[S02] C：变量与格式化输出
来源：http://ywd.xuetiantiany.cn

int a = 10; printf("%d\n", a);
来源：http://spf.yfazqb.com

[S03] C：读入整数
来源：http://yoi.pengpengdd.cyou

int x; scanf("%d", &x);
来源：http://kkd.hnxiangtu.top

[S04] C：字符串复制
来源：http://and.zhijiandao.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xoq.jinyuanbaomall.cn

[S05] C：字符串长度
来源：http://mai.fzhhl.top

strlen(s)
来源：http://qgy.yj202588.top

[S06] C：字符串比较
来源：http://lgs.cashguo.top

strcmp(a, b) == 0
来源：http://sfn.cheryme.top

[S07] C：数组遍历求和
来源：http://drs.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://szn.nwbrower.top

[S08] C：动态内存分配与释放
来源：http://hqb.0kj1m.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fxc.nanxuanxn.top

[S09] C：结构体定义与初始化
来源：http://jjg.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sak.yj20258.top

[S10] C：指针与解引用
来源：http://lkq.mhx1999.top

int *p = &a;  *p = 5;
来源：http://tns.kuanghao11.cn

[S11] C：逐行读文件
来源：http://gyn.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://pwo.dianchejie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://euw.yongpay.top

fclose(f);
来源：http://gmb.xylfe.cn

[S12] C：写文件
来源：http://fdt.snrcjt.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ulo.hesvh.cn

[S13] C：宏定义
来源：http://npi.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qzv.gaohongyu789.top

[S14] C：枚举
来源：http://ehr.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://kiw.ydzc1.top

[S15] C：类型转换
来源：http://cco.cheryme.top

(double) a / b
来源：http://vkk.gzhubu.top

[S16] C：位操作置位
来源：http://afu.kuanghao11.cn

x |= (1 << 3);
来源：http://ufi.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://wle.chenlongwang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vqx.zhoulong.xyz

[S18] C：命令行参数
来源：http://zsq.bjfxy.top

int main(int argc, char **argv)
来源：http://mgm.guowangkeji.top

[S19] C：快速排序
来源：http://dtq.uphjek.com

qsort(a, n, sizeof(int), cmp);
来源：http://xtm.pengpengdd.cyou

[S20] C：二分查找
来源：http://xwe.sufxvd.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dva.uphjek.com

[S21] C：字符类别判断
来源：http://ugk.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mpi.svipenyu.cn

[S22] C：字符串转数字
来源：http://rur.xingfuxueyuan.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://xfe.xuanzx.com

[S23] C：随机数
来源：http://trs.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gzn.zhongyouzk.top

[S24] C：获取本地时间
来源：http://xtl.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ptf.xuanzx.com

[S25] C：内存拷贝
来源：http://wge.fktsv.cn

memcpy(dst, src, n);
来源：http://hsj.gogol.net.cn

[S26] C：内存清零
来源：http://fgn.jianghu66.top

memset(a, 0, sizeof a);
来源：http://gcy.shangyingyoupin.top

[S27] C：定义常量
来源：http://zlr.aizwys.cn

const double PI = 3.14159;
来源：http://kra.pengpengdd.cyou

[S28] C：静态变量
来源：http://epv.zhengqikj.top

static int counter = 0;
来源：http://pdp.cashguo.top

[S29] C：变参函数
来源：http://isj.chenjidiqi.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pxv.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://ovs.ydjk.org.cn

#ifndef X_H
来源：http://nvp.ydjk.org.cn

#define X_H
来源：http://cgk.yuxming.cn

#endif
来源：http://bwa.nanxuanxn.top

[S31] C++：Hello World
来源：http://kos.yongpay.top

#include <iostream>
来源：http://cfh.fehbvm.com

int main() { std::cout << "Hello\n"; }
来源：http://pca.bbcook.cn

[S32] C++：字符串
来源：http://dvx.ybcxt.top

std::string s = "hi";  s += "!";
来源：http://fsl.gotoacloud.top

[S33] C++：vector 增删
来源：http://wst.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lnk.daxiang520.top

[S34] C++：遍历 vector
来源：http://poz.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://jue.yongpay.top

[S35] C++：map
来源：http://jyy.fehbvm.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://adx.wangshuangyany.cn

[S36] C++：unordered_map
来源：http://sbs.vehdjk.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ujz.yuxming.cn

[S37] C++：set
来源：http://stk.xingfuxueyuan.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dyd.yongpay.top

[S38] C++：排序
来源：http://uhp.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://pvc.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://srd.zhixingplan.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xfj.zhiwuduotai.top

[S40] C++：查找元素
来源：http://xzn.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lzh.fengsongda.top

[S41] C++：类与构造函数
来源：http://vmd.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xpj.gaohongyu789.top

[S42] C++：继承与虚函数
来源：http://kyj.zdqjudy.top

class B : public Base { public: void f() override {} };
来源：http://yos.yangfankeji.com

[S43] C++：智能指针
来源：http://fem.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://tnk.zycfv.cn

[S44] C++：引用传参
来源：http://chk.yuanzhike.top

void inc(int &x) { ++x; }
来源：http://nbn.xinyue.icu

[S45] C++：lambda
来源：http://owi.iojbl.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fbl.jyoumei.cn

[S46] C++：函数模板
来源：http://pxt.shangyingyoupin.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ret.shuidangran.top

[S47] C++：结构化绑定遍历
来源：http://kis.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kva.cdnleiting.top

[S48] C++：逐行读文件
来源：http://nca.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://ezc.hammf.cn

while (std::getline(in, line)) { }
来源：http://seh.zhongyouzk.top

[S49] C++：写文件
来源：http://ubs.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://prg.zhoulong.xyz

[S50] C++：格式化数字
来源：http://vof.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cys.uphjek.com

[S51] C++：显式类型转换
来源：http://dzj.jinqigufen.top

static_cast<double>(a) / b
来源：http://lif.zhixingplan.top

[S52] C++：const 与 noexcept
来源：http://zxe.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://efu.chenzaomai.com

[S53] C++：移动语义
来源：http://dzj.cucudq.cn

std::vector<int> w = std::move(v);
来源：http://pvw.havefunace.top

[S54] C++：异常处理
来源：http://wfp.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eyt.xingfuxueyuan.xyz

[S55] C++：结构化绑定
来源：http://jwp.smart0.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://fan.ywan-chungtsiang.top

[S56] C++：optional
来源：http://zdp.jinyuanbaomall.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fpq.zycfv.cn

[S57] C++：编译期常量
来源：http://oot.uphjek.com

constexpr int N = 10;
来源：http://yug.chenlongwang.top

[S58] C++：命名空间
来源：http://pjt.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://nwn.hongshengwenyu.top

[S59] C++：静态断言
来源：http://lvp.haohaochexian.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rkr.cqqwz.cn

[S60] C++：遍历并删除元素
来源：http://jks.tanke756.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://utd.andypj.xyz

================================================================================
来源：http://ipz.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nzl.meibo888.top

================================================================================
来源：http://bye.shuidangran.top

[T01] Kotlin：Hello World
来源：http://zzl.chenjidiqi.icu

println("Hello")
来源：http://eyq.tanke756.top

[T02] Kotlin：变量
来源：http://mli.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hkg.havefunace.top

[T03] Kotlin：字符串模板
来源：http://kxz.52xcode.cn

"值: $b"
来源：http://lps.hesvh.cn

[T04] Kotlin：空安全
来源：http://ede.yongpay.top

val n: String? = null;  n?.length
来源：http://zfc.yongpay.top

[T05] Kotlin：when 表达式
来源：http://qkk.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iff.pycfn.com

[T06] Kotlin：集合映射
来源：http://yrt.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dwq.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://dnm.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://llc.tianlin.xyz

[T08] Kotlin：数据类
来源：http://zpg.yj202588.top

data class User(val name: String, val age: Int)
来源：http://uea.hywenlv.cn

[T09] Kotlin：扩展函数
来源：http://bqx.fktsv.cn

fun String.exclaim() = this + "!"
来源：http://fir.zdqjudy.top

[T10] Kotlin：默认参数
来源：http://fjx.yueranfly.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nta.havefunace.top


<!-- 参考信息 -->