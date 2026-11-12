代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ybo.jinqigfzy.top

[R10] 正则匹配
来源：http://zbt.haohaochexian.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zjd.yuanzhike.top

[R11] case 多分支
来源：http://odh.cqqwz.cn

case "$1" in
来源：http://qdp.cucudq.cn

start) echo "启动" ;;
来源：http://slw.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://cld.havefunace.top

*)     echo "未知命令" ;;
来源：http://lpf.feifeiyinyue.top

esac
来源：http://ruv.sxryk.cn

[R12] for 遍历文件
来源：http://kkb.ivvv.top

for f in *.txt; do echo "$f"; done
来源：http://oro.dianchejie.cn

[R13] for 计数循环
来源：http://oid.bjfxy.top

for i in {1..10}; do echo "$i"; done
来源：http://aza.ppjwa.cn

[R14] C 风格 for
来源：http://lts.cucudq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rgg.yonumen.top

[R15] while 逐行读文件
来源：http://gtb.xuanzx.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aqm.hnxiangtu.top

[R16] until 等待条件
来源：http://svp.jqgufenzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://okj.9152youxi.cn

[R17] 数组定义与取值
来源：http://lyd.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lnh.yangfankeji.com

[R18] 遍历数组
来源：http://xna.redwolf501.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eud.chenzaomai.com

[R19] 数组长度
来源：http://qmf.hesvh.cn

echo "${#arr[@]}"
来源：http://kvl.yj20258888.top

[R20] 关联数组（字典）
来源：http://lro.shzxlz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ryf.haohaochexian.top

[R21] 字符串长度
来源：http://afj.yuxming.cn

echo "${#s}"
来源：http://vio.gotoacloud.top

[R22] 截取子串
来源：http://tbz.zhongyouzk.top

echo "${s:0:5}"
来源：http://yxv.kuanghao11.cn

[R23] 字符串替换
来源：http://qvr.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pma.9152youxi.cn

[R24] 大小写转换
来源：http://ove.kuanghao11.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ulw.zhoulong.xyz

[R25] 去后缀 / 去前缀
来源：http://gww.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ouc.zhixingplan.top

[R26] 命令替换
来源：http://arp.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://wic.zdbjq.cn

[R27] 算术展开
来源：http://caa.quarkkingdee.top

echo $((1 + 2 * 3))
来源：http://hot.zycfv.cn

[R28] 浮点运算
来源：http://pnv.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://kxo.zhiwuduotai.top

[R29] 定义函数
来源：http://fiz.zhiwuduotai.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lwp.yfazqb.com

[R30] 函数返回状态码
来源：http://pbo.jqgfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://rgq.daria6918.cn

[R31] 局部变量
来源：http://tmw.xuetiantiany.cn

f() { local x=1; echo "$x"; }
来源：http://lqq.yueranfly.top

[R32] 参数个数校验
来源：http://euy.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tjg.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://yur.ctjpmb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wqh.jinghuilouyu.cn

[R34] 退出时清理
来源：http://rfd.shangyingyoupin.top

trap 'rm -f "$tmp"' EXIT
来源：http://adg.shzxlz.cn

[R35] 后台执行并等待
来源：http://gju.cqqwz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jte.zhixingplan.top

[R36] 并发执行多个任务
来源：http://jhy.hongshengwenyu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://brh.chenlongwang.top

[R37] 把输出赋给变量
来源：http://rox.havefunace.top

files=$(ls -1)
来源：http://gfi.haohaochexian.top

[R38] 管道串联
来源：http://wlu.sysykeji.top

cat a.txt | grep -i error | wc -l
来源：http://kav.nanxuanxn.top

[R39] 重定向标准输出与错误
来源：http://vie.hfpthk.cn

cmd > out.log 2>&1
来源：http://nql.zycfv.cn

[R40] 追加写日志
来源：http://zqb.chenzaomai.com

echo "log" >> out.log
来源：http://obl.jqgufenzy.top

[R41] 丢弃输出
来源：http://tvt.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://mef.yfazqb.com

[R42] 输入重定向
来源：http://qve.yj20258888.top

wc -l < a.txt
来源：http://ypw.bjfxy.top

[R43] 按名字查找文件
来源：http://mzw.shangyingyoupin.top

find . -name "*.log" -type f
来源：http://xwa.zhijiandao.cn

[R44] 按修改时间查找
来源：http://lpk.haohaochexian.top

find . -mtime -7 -type f
来源：http://ydd.hywenlv.cn

[R45] 批量删除
来源：http://zrr.jinqigfzy.top

find . -name "*.tmp" -delete
来源：http://svt.bbcook.cn

[R46] 递归替换文件内容
来源：http://fls.gzhubu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sjr.aibaodan.cn

[R47] sed 单行替换
来源：http://amp.meibo888.top

sed -i 's/foo/bar/g' a.txt
来源：http://kll.jinqigufen.top

[R48] awk 取指定列
来源：http://xku.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://bjy.jinqigufen.top

[R49] awk 带条件
来源：http://ynx.yangfankeji.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hvt.uphjek.com

[R50] awk 求和
来源：http://pgd.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vcs.vqdsnc.cn

[R51] 排序去重取前几
来源：http://csp.cqqwz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nhn.yfazqb.com

[R52] 统计行数
来源：http://ysg.wangdashe.top

wc -l a.txt
来源：http://zic.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://fqu.zhongyouzk.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lap.dashuyun.cn

[R54] 比较两个文件
来源：http://vkj.mhx1999.top

diff a.txt b.txt
来源：http://gyr.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://dua.smart0.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cgn.tanke756.top

[R56] 远程拷贝
来源：http://qrf.andypj.xyz

scp file user@host:/path/
来源：http://xfa.mhx1999.top

[R57] 远程执行命令
来源：http://ygm.feifeiyinyue.top

ssh user@host 'uptime'
来源：http://zxh.jinqigfzy.top

[R58] 下载文件
来源：http://nhc.yuxming.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qpg.vehdjk.com

[R59] 发 POST JSON
来源：http://ldo.zhaomingkeji.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gwe.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://txp.snrcjt.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eeo.yonumen.top

[R61] 磁盘占用
来源：http://mgv.feifeiyinyue.top

df -h;  du -sh *
来源：http://doc.chenzaomai.com

[R62] 找最占空间的文件
来源：http://myv.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://hbi.fzhhl.top

[R63] 内存与进程
来源：http://nks.hongshengwenyu.top

free -h;  ps aux | grep nginx
来源：http://emr.zhaomingkeji.xyz

[R64] 结束进程
来源：http://nbz.aizwys.cn

kill -9 $(pgrep -f app.py)
来源：http://abp.bjfxy.top

[R65] 查看端口占用
来源：http://vwm.xylfe.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zin.sysykeji.top

[R66] 定时任务
来源：http://ple.daria6918.cn

crontab -e;  crontab -l
来源：http://csz.sufxvd.cn

[R67] 生成随机十六进制串
来源：http://bqh.c1oappe.top

openssl rand -hex 16
来源：http://lws.fehbvm.com

[R68] 计算文件校验值
来源：http://sug.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ljt.xylfe.cn

[R69] 生成随机密码
来源：http://duz.epnwcf.com

head -c 16 /dev/urandom | base64
来源：http://qcn.zdbjq.cn

[R70] 时间戳与互转
来源：http://tjs.jinghuilouyu.cn

date +%s;  date -d @1700000000
来源：http://rjk.ybcxt.top

[R71] 日期格式化
来源：http://pbw.sweek.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vyb.fehbvm.com

[R72] 等待端口就绪
来源：http://xix.ppjwa.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://coc.cashguo.top

[R73] 分割大日志
来源：http://drc.redwolf501.top

split -l 1000 big.log part_
来源：http://rxz.yuxming.cn

[R74] 批量重命名
来源：http://ern.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jyf.nanxuanxn.top

[R75] 导出环境变量
来源：http://kfg.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://dec.zdbjq.cn

[R76] 使用临时文件
来源：http://dbt.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://trh.shanyushiyangtech.top

[R77] 读取用户输入
来源：http://gpx.jqgufenzy.top

read -rp "请输入: " ans
来源：http://osp.jqgfzy.top

[R78] 交互式菜单
来源：http://zic.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gwh.sweek.top

[R79] 解析命令行选项
来源：http://zuc.hnqzz.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mnj.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://wlf.aizwys.cn

time ./run.sh
来源：http://win.jyoumei.cn

================================================================================
来源：http://otz.hfpthk.cn

S. C / C++ 专题
来源：http://fgs.cashguo.top

================================================================================
来源：http://pqz.hysaishi.cn

[S01] C：Hello World
来源：http://oja.redwolf501.top

#include <stdio.h>
来源：http://ypc.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ubu.shanyushiyangkeji.top

[S02] C：变量与格式化输出
来源：http://yzv.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://azq.sxryk.cn

[S03] C：读入整数
来源：http://uxn.shuidangran.top

int x; scanf("%d", &x);
来源：http://ths.zdqjudy.top

[S04] C：字符串复制
来源：http://ipw.jiagoushi.top

char dst[32]; strcpy(dst, "hi");
来源：http://rxn.andypj.xyz

[S05] C：字符串长度
来源：http://xrp.zhoulong.xyz

strlen(s)
来源：http://tag.zdqjudy.top

[S06] C：字符串比较
来源：http://kqn.sxryk.cn

strcmp(a, b) == 0
来源：http://zrc.vehdjk.com

[S07] C：数组遍历求和
来源：http://vqs.316326.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nlo.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://rhe.0kj1m.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xtu.shanyushiyangkeji.top

[S09] C：结构体定义与初始化
来源：http://yil.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yqk.tanke756.top

[S10] C：指针与解引用
来源：http://vsz.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://wel.chenlongwang.top

[S11] C：逐行读文件
来源：http://mbz.epnwcf.com

FILE *f = fopen("a.txt", "r");
来源：http://ibl.cheryme.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://chy.hnxiangtu.top

fclose(f);
来源：http://esl.yuanzhike.top

[S12] C：写文件
来源：http://jcr.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vlk.aibaodan.cn

[S13] C：宏定义
来源：http://qav.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fas.cucudq.cn

[S14] C：枚举
来源：http://res.quarkkingdee.top

enum Color { RED, GREEN, BLUE };
来源：http://qls.dianchejie.cn

[S15] C：类型转换
来源：http://hns.ctjpmb.com

(double) a / b
来源：http://mzf.svipenyu.cn

[S16] C：位操作置位
来源：http://cjo.smart0.xyz

x |= (1 << 3);
来源：http://coi.fehbvm.com

[S17] C：安全拼接字符串
来源：http://eub.mhx1999.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zog.jqgfzy.top

[S18] C：命令行参数
来源：http://qbh.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://nzs.feifeiyinyue.top

[S19] C：快速排序
来源：http://yvz.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://vxv.havefunace.top

[S20] C：二分查找
来源：http://uyd.feifeiyinyue.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tga.zhixingplan.top

[S21] C：字符类别判断
来源：http://hay.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oef.bbcook.cn

[S22] C：字符串转数字
来源：http://xtu.xingfuxueyuan.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://vzl.zhijiandao.cn

[S23] C：随机数
来源：http://avy.tian-w.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pku.sjlbkw.cn

[S24] C：获取本地时间
来源：http://qlk.zhixingplan.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://idr.gaohongyu789.top

[S25] C：内存拷贝
来源：http://czb.chenzaomai.com

memcpy(dst, src, n);
来源：http://tky.fengsongda.top

[S26] C：内存清零
来源：http://sbz.c1oappe.top

memset(a, 0, sizeof a);
来源：http://uve.sweek.top

[S27] C：定义常量
来源：http://ckt.gzhubu.top

const double PI = 3.14159;
来源：http://iwp.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://hyy.ydjk.org.cn

static int counter = 0;
来源：http://ucq.tianlin.xyz

[S29] C：变参函数
来源：http://swj.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ifd.sysykeji.top

[S30] C：头文件保护
来源：http://kap.smart0.xyz

#ifndef X_H
来源：http://iso.9152youxi.cn

#define X_H
来源：http://fwd.zhoulong.xyz

#endif
来源：http://jjh.yonumen.top

[S31] C++：Hello World
来源：http://ret.nanxuanxn.top

#include <iostream>
来源：http://rgn.epnwcf.com

int main() { std::cout << "Hello\n"; }
来源：http://vvc.0kj1m.cn

[S32] C++：字符串
来源：http://nzg.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://lev.ppjwa.cn

[S33] C++：vector 增删
来源：http://odg.ydzc1.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ggt.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://pzv.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://bew.jiagoushi.top

[S35] C++：map
来源：http://uhs.tarul.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jpt.zhongyouzk.top

[S36] C++：unordered_map
来源：http://bzs.jiagoushi.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tua.meibo888.top

[S37] C++：set
来源：http://faa.xuanzx.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://thc.tianlin.xyz

[S38] C++：排序
来源：http://lbu.52xcode.cn

std::sort(v.begin(), v.end());
来源：http://gll.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://bxi.yj20258888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://liy.hongshengwenyu.top

[S40] C++：查找元素
来源：http://muy.tarul.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cbq.hysaishi.cn

[S41] C++：类与构造函数
来源：http://tjj.fanxiaobao.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iwc.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://tim.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://gcq.zycfv.cn

[S43] C++：智能指针
来源：http://vpv.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://paj.pengpengdd.cyou

[S44] C++：引用传参
来源：http://cju.cheryme.top

void inc(int &x) { ++x; }
来源：http://vvf.sufxvd.cn

[S45] C++：lambda
来源：http://kzs.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://irt.hfpthk.cn

[S46] C++：函数模板
来源：http://lit.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gft.316326.xyz

[S47] C++：结构化绑定遍历
来源：http://wnl.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://koa.hammf.cn

[S48] C++：逐行读文件
来源：http://ciw.yongpay.top

std::ifstream in("a.txt");  std::string line;
来源：http://nys.bbcook.cn

while (std::getline(in, line)) { }
来源：http://ahs.sweek.top

[S49] C++：写文件
来源：http://txw.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jqa.hnqzz.top

[S50] C++：格式化数字
来源：http://wiz.svipenyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pha.vehdjk.com

[S51] C++：显式类型转换
来源：http://dqq.jinyuanbaomall.cn

static_cast<double>(a) / b
来源：http://ezi.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://kku.jyoumei.cn

int size() const noexcept { return n_; }
来源：http://psu.iojbl.cn

[S53] C++：移动语义
来源：http://dvl.shanyushiyangtech.top

std::vector<int> w = std::move(v);
来源：http://zmk.fehbvm.com

[S54] C++：异常处理
来源：http://xlk.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dbd.shuidangran.top

[S55] C++：结构化绑定
来源：http://twp.iojbl.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ciq.guannengcc.top

[S56] C++：optional
来源：http://hzr.sxryk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xzv.dianchejie.cn

[S57] C++：编译期常量
来源：http://krd.yj202588.top

constexpr int N = 10;
来源：http://odp.uphjek.com

[S58] C++：命名空间
来源：http://tnm.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://dmy.uphjek.com

[S59] C++：静态断言
来源：http://pqp.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ksn.daxiang520.top

[S60] C++：遍历并删除元素
来源：http://uje.tian-w.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qll.shangyingyoupin.top

================================================================================
来源：http://ixb.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qrk.dashuyun.cn

================================================================================
来源：http://oew.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://fyu.yj20258.top

println("Hello")
来源：http://mde.fengsongda.top

[T02] Kotlin：变量
来源：http://hsw.chenlongwang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ztj.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://iae.sweek.top

"值: $b"
来源：http://vxk.yonumen.top

[T04] Kotlin：空安全
来源：http://kuj.cheryme.top

val n: String? = null;  n?.length
来源：http://gnl.zhengqikj.top

[T05] Kotlin：when 表达式
来源：http://dvi.guowangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://deg.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://uan.fengsongda.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bmh.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://kna.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ewc.zhixingplan.top

[T08] Kotlin：数据类
来源：http://kik.yonumen.top

data class User(val name: String, val age: Int)
来源：http://fnw.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://gpx.zhengqikj.top

fun String.exclaim() = this + "!"
来源：http://lsy.tian-w.cn

[T10] Kotlin：默认参数
来源：http://mio.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gqz.guowangkeji.top


<!-- 参考信息 -->