代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pzk.yonumen.top

[R10] 正则匹配
来源：http://azv.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nsw.zhixingplan.top

[R11] case 多分支
来源：http://sks.quarkkingdee.top

case "$1" in
来源：http://dbz.epnwcf.com

start) echo "启动" ;;
来源：http://lrl.shuidangran.top

stop)  echo "停止" ;;
来源：http://izp.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://bmp.ydjk.org.cn

esac
来源：http://tsc.birdmap.top

[R12] for 遍历文件
来源：http://iwf.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://wjn.sufxvd.cn

[R13] for 计数循环
来源：http://bva.tarul.cn

for i in {1..10}; do echo "$i"; done
来源：http://ubg.yonumen.top

[R14] C 风格 for
来源：http://qkp.zhijiandao.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tpg.wangshuangyany.cn

[R15] while 逐行读文件
来源：http://zic.zycfv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mez.yfazqb.com

[R16] until 等待条件
来源：http://uck.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rth.kuanghao11.cn

[R17] 数组定义与取值
来源：http://xyx.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://nya.yfazqb.com

[R18] 遍历数组
来源：http://jxh.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bts.svipenyu.cn

[R19] 数组长度
来源：http://gyd.jyoumei.cn

echo "${#arr[@]}"
来源：http://gvo.cashguo.top

[R20] 关联数组（字典）
来源：http://qxd.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bvu.hfpthk.cn

[R21] 字符串长度
来源：http://cps.yueranfly.top

echo "${#s}"
来源：http://kpb.ydzc1.top

[R22] 截取子串
来源：http://dgx.hysaishi.cn

echo "${s:0:5}"
来源：http://uht.yj20258888.top

[R23] 字符串替换
来源：http://xhk.bbcook.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uwp.cdnleiting.top

[R24] 大小写转换
来源：http://tns.52xcode.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vye.epnwcf.com

[R25] 去后缀 / 去前缀
来源：http://djq.9152youxi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bwb.wangshuangyany.cn

[R26] 命令替换
来源：http://rnz.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://ikw.epnwcf.com

[R27] 算术展开
来源：http://ixl.jinyuanbaomall.cn

echo $((1 + 2 * 3))
来源：http://mln.yuanzhike.top

[R28] 浮点运算
来源：http://wbs.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://ncj.yongpay.top

[R29] 定义函数
来源：http://zqn.chenzaomai.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ozz.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://cas.dianchejie.cn

f() { return 0; }; f || echo "失败了"
来源：http://mwt.smart0.xyz

[R31] 局部变量
来源：http://tje.jiagoushi.top

f() { local x=1; echo "$x"; }
来源：http://ems.iojbl.cn

[R32] 参数个数校验
来源：http://scr.jyoumei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://twz.aibaodan.cn

[R33] 捕获错误并提示行号
来源：http://lix.yvedp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xma.mhx1999.top

[R34] 退出时清理
来源：http://wvi.uphjek.com

trap 'rm -f "$tmp"' EXIT
来源：http://lop.hesvh.cn

[R35] 后台执行并等待
来源：http://cfd.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mki.sweek.top

[R36] 并发执行多个任务
来源：http://eks.dianchejie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qql.jqgfzy.top

[R37] 把输出赋给变量
来源：http://wcd.hysaishi.cn

files=$(ls -1)
来源：http://uir.sweek.top

[R38] 管道串联
来源：http://ypu.jqgufenzy.top

cat a.txt | grep -i error | wc -l
来源：http://arq.epnwcf.com

[R39] 重定向标准输出与错误
来源：http://yad.dianchejie.cn

cmd > out.log 2>&1
来源：http://cvo.sweek.top

[R40] 追加写日志
来源：http://cso.chenjidiqi.icu

echo "log" >> out.log
来源：http://hya.shuidangran.top

[R41] 丢弃输出
来源：http://zre.zhengqikj.top

cmd >/dev/null 2>&1
来源：http://duy.fanxiaobao.xyz

[R42] 输入重定向
来源：http://iun.xylfe.cn

wc -l < a.txt
来源：http://zce.yfazqb.com

[R43] 按名字查找文件
来源：http://xot.hcnkem.com

find . -name "*.log" -type f
来源：http://elh.hnxiangtu.top

[R44] 按修改时间查找
来源：http://lwe.uphjek.com

find . -mtime -7 -type f
来源：http://guy.hongshengwenyu.top

[R45] 批量删除
来源：http://tdz.fktsv.cn

find . -name "*.tmp" -delete
来源：http://hga.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://hte.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pei.tanke756.top

[R47] sed 单行替换
来源：http://end.xingfuxueyuan.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://ymg.fehbvm.com

[R48] awk 取指定列
来源：http://lrs.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://yxy.meibo888.top

[R49] awk 带条件
来源：http://oam.zhiwuduotai.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jqv.tanke756.top

[R50] awk 求和
来源：http://rfg.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://qwv.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://nbw.yangfankeji.com

sort a.txt | uniq -c | sort -rn | head
来源：http://hyl.yongpay.top

[R52] 统计行数
来源：http://fai.feifeiyinyue.top

wc -l a.txt
来源：http://onb.wangshuangyany.cn

[R53] 查看文件头与实时尾
来源：http://gcg.tianlin.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wpy.meibo888.top

[R54] 比较两个文件
来源：http://xwq.nwbrower.top

diff a.txt b.txt
来源：http://mnq.ybcxt.top

[R55] 压缩与解压
来源：http://naj.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cbd.cashguo.top

[R56] 远程拷贝
来源：http://qvg.52xcode.cn

scp file user@host:/path/
来源：http://qxz.yj20258.top

[R57] 远程执行命令
来源：http://kku.xziqi.cn

ssh user@host 'uptime'
来源：http://wra.52xcode.cn

[R58] 下载文件
来源：http://fwo.haohaochexian.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lze.guannengcc.top

[R59] 发 POST JSON
来源：http://fdo.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wzc.zhengqikj.top

[R60] 只看 HTTP 状态码
来源：http://vqe.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xen.yuanzhike.top

[R61] 磁盘占用
来源：http://wwd.tanke756.top

df -h;  du -sh *
来源：http://kqu.zycfv.cn

[R62] 找最占空间的文件
来源：http://vke.cdnleiting.top

du -ah . | sort -rh | head -10
来源：http://gie.jinghuilouyu.cn

[R63] 内存与进程
来源：http://jdy.bbcook.cn

free -h;  ps aux | grep nginx
来源：http://mqw.redwolf501.top

[R64] 结束进程
来源：http://cqp.jianghu66.top

kill -9 $(pgrep -f app.py)
来源：http://qrk.quarkkingdee.top

[R65] 查看端口占用
来源：http://ksl.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xjc.chenlongwang.top

[R66] 定时任务
来源：http://tnb.nwbrower.top

crontab -e;  crontab -l
来源：http://ixa.birdmap.top

[R67] 生成随机十六进制串
来源：http://zhm.xuetiantiany.cn

openssl rand -hex 16
来源：http://cjo.jiagoushi.top

[R68] 计算文件校验值
来源：http://naz.sxryk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://inc.jlsjyb.cn

[R69] 生成随机密码
来源：http://yop.zhongyouzk.top

head -c 16 /dev/urandom | base64
来源：http://jbf.xylfe.cn

[R70] 时间戳与互转
来源：http://qww.52xcode.cn

date +%s;  date -d @1700000000
来源：http://cdi.ydjk.org.cn

[R71] 日期格式化
来源：http://cdw.nanxuanxn.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fqs.sysykeji.top

[R72] 等待端口就绪
来源：http://xuc.hnxiangtu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lit.cqqwz.cn

[R73] 分割大日志
来源：http://zhq.bbcook.cn

split -l 1000 big.log part_
来源：http://wtm.jlsjyb.cn

[R74] 批量重命名
来源：http://lzi.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://odk.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://ckk.gzhubu.top

export PATH="$HOME/bin:$PATH"
来源：http://pka.c1oappe.top

[R76] 使用临时文件
来源：http://awn.fzhhl.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vwy.wangdashe.top

[R77] 读取用户输入
来源：http://uxt.iojbl.cn

read -rp "请输入: " ans
来源：http://tnf.svipenyu.cn

[R78] 交互式菜单
来源：http://kzo.316326.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://eud.xingfuxueyuan.xyz

[R79] 解析命令行选项
来源：http://azn.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uim.jianghu66.top

[R80] 查看脚本执行耗时
来源：http://jay.zycfv.cn

time ./run.sh
来源：http://qkj.zdqjudy.top

================================================================================
来源：http://jxw.fzhhl.top

S. C / C++ 专题
来源：http://xlc.bjfxy.top

================================================================================
来源：http://wti.gotoacloud.top

[S01] C：Hello World
来源：http://xit.mhx1999.top

#include <stdio.h>
来源：http://bft.hcnkem.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://pwk.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://bgy.9152youxi.cn

int a = 10; printf("%d\n", a);
来源：http://slf.snrcjt.cn

[S03] C：读入整数
来源：http://nlj.gogol.net.cn

int x; scanf("%d", &x);
来源：http://yok.daria6918.cn

[S04] C：字符串复制
来源：http://njk.shzxlz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tyg.birdmap.top

[S05] C：字符串长度
来源：http://nxh.redwolf501.top

strlen(s)
来源：http://ncg.gaohongyu789.top

[S06] C：字符串比较
来源：http://fqq.birdmap.top

strcmp(a, b) == 0
来源：http://jja.sufxvd.cn

[S07] C：数组遍历求和
来源：http://oay.pengpengdd.cyou

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qsd.havefunace.top

[S08] C：动态内存分配与释放
来源：http://xai.ybcxt.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://azx.cdnleiting.top

[S09] C：结构体定义与初始化
来源：http://xhx.birdmap.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yrj.nanxinkj.top

[S10] C：指针与解引用
来源：http://rrb.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://ufr.daxiang520.top

[S11] C：逐行读文件
来源：http://jcp.uphjek.com

FILE *f = fopen("a.txt", "r");
来源：http://ipa.ydjk.org.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fir.yuxming.cn

fclose(f);
来源：http://zip.jiagoushi.top

[S12] C：写文件
来源：http://urw.gaohongyu789.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://snm.wangdashe.top

[S13] C：宏定义
来源：http://zye.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yrz.jinyuanbaomall.cn

[S14] C：枚举
来源：http://lgn.wangshuangyany.cn

enum Color { RED, GREEN, BLUE };
来源：http://svn.jinghuilouyu.cn

[S15] C：类型转换
来源：http://ioa.cashguo.top

(double) a / b
来源：http://dfo.cashguo.top

[S16] C：位操作置位
来源：http://wag.jqgfzy.top

x |= (1 << 3);
来源：http://mds.shangyingyoupin.top

[S17] C：安全拼接字符串
来源：http://nyo.tianlin.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iln.nanxinkj.top

[S18] C：命令行参数
来源：http://tbp.xinyue.icu

int main(int argc, char **argv)
来源：http://arf.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://fit.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://shg.shanyushiyangtech.top

[S20] C：二分查找
来源：http://ckm.zhijiandao.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jlc.daxiang520.top

[S21] C：字符类别判断
来源：http://sjo.xinyue.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kxn.jqgfzy.top

[S22] C：字符串转数字
来源：http://bys.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://kzi.daria6918.cn

[S23] C：随机数
来源：http://yrg.hywenlv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ouf.gogol.net.cn

[S24] C：获取本地时间
来源：http://rse.xuanzx.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jfl.epnwcf.com

[S25] C：内存拷贝
来源：http://muv.xziqi.cn

memcpy(dst, src, n);
来源：http://nma.ybcxt.top

[S26] C：内存清零
来源：http://jrt.mhx1999.top

memset(a, 0, sizeof a);
来源：http://dsr.jiagoushi.top

[S27] C：定义常量
来源：http://jfg.zycfv.cn

const double PI = 3.14159;
来源：http://hzz.gogol.net.cn

[S28] C：静态变量
来源：http://mks.nanxuanxn.top

static int counter = 0;
来源：http://utl.hongshengwenyu.top

[S29] C：变参函数
来源：http://wdr.yanxiufei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://huz.gogol.net.cn

[S30] C：头文件保护
来源：http://ldn.gzhubu.top

#ifndef X_H
来源：http://tyn.tian-w.cn

#define X_H
来源：http://osl.vqdsnc.cn

#endif
来源：http://tal.fzhhl.top

[S31] C++：Hello World
来源：http://dnb.nanxinkj.top

#include <iostream>
来源：http://jwk.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://tnb.yj20258.top

[S32] C++：字符串
来源：http://oqe.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://pmn.52xcode.cn

[S33] C++：vector 增删
来源：http://qux.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iij.jinyuanbaomall.cn

[S34] C++：遍历 vector
来源：http://wxc.yongpay.top

for (auto &x : v) { std::cout << x; }
来源：http://prc.0kj1m.cn

[S35] C++：map
来源：http://xax.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ywq.tian-w.cn

[S36] C++：unordered_map
来源：http://rhj.ybcxt.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sgr.feifeiyinyue.top

[S37] C++：set
来源：http://wem.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dxk.yanxiufei.cn

[S38] C++：排序
来源：http://gzi.hnqzz.top

std::sort(v.begin(), v.end());
来源：http://rkc.meibo888.top

[S39] C++：自定义比较器排序
来源：http://vcd.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://auv.tianlin.xyz

[S40] C++：查找元素
来源：http://kte.wangdashe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ulu.sufxvd.cn

[S41] C++：类与构造函数
来源：http://xjr.meibo888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rsk.zhengqikj.top

[S42] C++：继承与虚函数
来源：http://uwc.mhx1999.top

class B : public Base { public: void f() override {} };
来源：http://tyf.ywan-chungtsiang.top

[S43] C++：智能指针
来源：http://klh.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://cxy.shanyushiyangkeji.top

[S44] C++：引用传参
来源：http://wih.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://hwa.guannengcc.top

[S45] C++：lambda
来源：http://hzz.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://gxd.tian-w.cn

[S46] C++：函数模板
来源：http://bkc.ydzc1.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jdv.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://ohm.hfpthk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kpa.nwbrower.top

[S48] C++：逐行读文件
来源：http://gis.zdbjq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ite.chenzaomai.com

while (std::getline(in, line)) { }
来源：http://lus.tarul.cn

[S49] C++：写文件
来源：http://erw.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ngp.ivvv.top

[S50] C++：格式化数字
来源：http://erk.tianlin.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vuc.zdqjudy.top

[S51] C++：显式类型转换
来源：http://xsi.jinqigufen.top

static_cast<double>(a) / b
来源：http://aog.hfpthk.cn

[S52] C++：const 与 noexcept
来源：http://ixz.ivvv.top

int size() const noexcept { return n_; }
来源：http://wut.nanxuanxn.top

[S53] C++：移动语义
来源：http://ivd.svipenyu.cn

std::vector<int> w = std::move(v);
来源：http://lhn.yj20258888.top

[S54] C++：异常处理
来源：http://rgx.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ysm.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://vuj.cheryme.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gvi.yueranfly.top

[S56] C++：optional
来源：http://mwh.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ege.ydjk.org.cn

[S57] C++：编译期常量
来源：http://hwf.jyoumei.cn

constexpr int N = 10;
来源：http://eij.gaohongyu789.top

[S58] C++：命名空间
来源：http://vvb.uphjek.com

namespace ns { int f() { return 1; } }
来源：http://xow.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://ofv.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kpw.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://wsp.xuetiantiany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lry.zhongyouzk.top

================================================================================
来源：http://hoh.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kvp.jqgufenzy.top

================================================================================
来源：http://bsq.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://oov.daria6918.cn

println("Hello")
来源：http://dts.svipenyu.cn

[T02] Kotlin：变量
来源：http://gnq.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rvf.svipenyu.cn

[T03] Kotlin：字符串模板
来源：http://vql.jianghu66.top

"值: $b"
来源：http://vas.tarul.cn

[T04] Kotlin：空安全
来源：http://wys.daxiang520.top

val n: String? = null;  n?.length
来源：http://wuk.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://uxj.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ztc.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://yke.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://fpi.pengpengdd.cyou

[T07] Kotlin：集合过滤
来源：http://ttv.shanyushiyangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bgv.zhaomingkeji.xyz

[T08] Kotlin：数据类
来源：http://urn.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://ttc.xingfuxueyuan.xyz

[T09] Kotlin：扩展函数
来源：http://qvw.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://jdb.gzhubu.top

[T10] Kotlin：默认参数
来源：http://zcw.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ldv.aizwys.cn


<!-- 参考信息 -->