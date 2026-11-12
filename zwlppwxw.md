代发 wailian999

name="${1:-default}"
来源：http://ptf.tian-w.cn

[R06] 判断命令是否存在
来源：http://gbw.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gml.aizwys.cn

[R07] if 判断文件
来源：http://gqr.yongpay.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jsv.yueranfly.top

[R08] 数值比较
来源：http://ynn.jinqigufen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qus.fehbvm.com

[R09] 字符串比较
来源：http://rrl.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://emc.yanxiufei.cn

[R10] 正则匹配
来源：http://tyb.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dws.sxryk.cn

[R11] case 多分支
来源：http://rex.haohaochexian.top

case "$1" in
来源：http://dgx.aibaodan.cn

start) echo "启动" ;;
来源：http://kho.zhiwuduotai.top

stop)  echo "停止" ;;
来源：http://ymt.ivvv.top

*)     echo "未知命令" ;;
来源：http://mdn.hesvh.cn

esac
来源：http://drm.yongpay.top

[R12] for 遍历文件
来源：http://mmi.feifeiyinyue.top

for f in *.txt; do echo "$f"; done
来源：http://sps.chenzaomai.com

[R13] for 计数循环
来源：http://sfl.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://ena.tarul.cn

[R14] C 风格 for
来源：http://ool.shanyushiyangtech.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://utb.snrcjt.cn

[R15] while 逐行读文件
来源：http://qba.tanke756.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vsz.yongpay.top

[R16] until 等待条件
来源：http://tyv.316326.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vfa.tarul.cn

[R17] 数组定义与取值
来源：http://fhi.dashuyun.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dgv.zhiwuduotai.top

[R18] 遍历数组
来源：http://irs.sysykeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wit.gogol.net.cn

[R19] 数组长度
来源：http://dsx.birdmap.top

echo "${#arr[@]}"
来源：http://tsw.pycfn.com

[R20] 关联数组（字典）
来源：http://ewg.ehwqpu.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mzb.birdmap.top

[R21] 字符串长度
来源：http://vcr.jinghuilouyu.cn

echo "${#s}"
来源：http://lks.wangshuangyany.cn

[R22] 截取子串
来源：http://xed.zhaomingkeji.xyz

echo "${s:0:5}"
来源：http://hmz.jianghu66.top

[R23] 字符串替换
来源：http://zur.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cwl.hfpthk.cn

[R24] 大小写转换
来源：http://wsm.nwbrower.top

echo "${s^^}"; echo "${s,,}"
来源：http://pnf.mhx1999.top

[R25] 去后缀 / 去前缀
来源：http://pyv.guowangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mjs.jinqigfzy.top

[R26] 命令替换
来源：http://xbg.yuxming.cn

now=$(date +%F); echo "$now"
来源：http://bsr.jqgufenzy.top

[R27] 算术展开
来源：http://wtn.epnwcf.com

echo $((1 + 2 * 3))
来源：http://yqv.ybcxt.top

[R28] 浮点运算
来源：http://xmo.birdmap.top

echo "scale=2; 10/3" | bc
来源：http://kzk.hongshengwenyu.top

[R29] 定义函数
来源：http://wza.zycfv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://edg.0kj1m.cn

[R30] 函数返回状态码
来源：http://nax.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://ntj.guannengcc.top

[R31] 局部变量
来源：http://rhw.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://hmr.wangdashe.top

[R32] 参数个数校验
来源：http://qgq.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iby.zdqjudy.top

[R33] 捕获错误并提示行号
来源：http://tsw.jiagoushi.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lzx.zdbjq.cn

[R34] 退出时清理
来源：http://cbd.zycfv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://izs.aibaodan.cn

[R35] 后台执行并等待
来源：http://wrs.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://idg.birdmap.top

[R36] 并发执行多个任务
来源：http://lou.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sip.zhaomingkeji.xyz

[R37] 把输出赋给变量
来源：http://knw.xylfe.cn

files=$(ls -1)
来源：http://hik.pycfn.com

[R38] 管道串联
来源：http://cmq.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://nou.jinyuanbaomall.cn

[R39] 重定向标准输出与错误
来源：http://qyf.ydjk.org.cn

cmd > out.log 2>&1
来源：http://ahc.shuidangran.top

[R40] 追加写日志
来源：http://dir.zdqjudy.top

echo "log" >> out.log
来源：http://fjp.cqqwz.cn

[R41] 丢弃输出
来源：http://zwt.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://szb.uphjek.com

[R42] 输入重定向
来源：http://rfa.tianlin.xyz

wc -l < a.txt
来源：http://zoa.yuxming.cn

[R43] 按名字查找文件
来源：http://eui.pengpengdd.cyou

find . -name "*.log" -type f
来源：http://wpe.bbcook.cn

[R44] 按修改时间查找
来源：http://epj.aizwys.cn

find . -mtime -7 -type f
来源：http://sbb.gaohongyu789.top

[R45] 批量删除
来源：http://baq.sufxvd.cn

find . -name "*.tmp" -delete
来源：http://umu.zdqjudy.top

[R46] 递归替换文件内容
来源：http://pdt.yongpay.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uof.cheryme.top

[R47] sed 单行替换
来源：http://ouv.yj20258.top

sed -i 's/foo/bar/g' a.txt
来源：http://qzb.epnwcf.com

[R48] awk 取指定列
来源：http://xjh.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://gqd.yongpay.top

[R49] awk 带条件
来源：http://pak.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yjm.quarkkingdee.top

[R50] awk 求和
来源：http://nvs.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://wcb.iojbl.cn

[R51] 排序去重取前几
来源：http://ius.yj20258888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://uhc.zhengqikj.top

[R52] 统计行数
来源：http://blf.jqgufenzy.top

wc -l a.txt
来源：http://pbe.pengpengdd.cyou

[R53] 查看文件头与实时尾
来源：http://eol.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uvl.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://ibh.jinghuilouyu.cn

diff a.txt b.txt
来源：http://abl.wangdashe.top

[R55] 压缩与解压
来源：http://cpz.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ljg.svipenyu.cn

[R56] 远程拷贝
来源：http://tej.nanxuanxn.top

scp file user@host:/path/
来源：http://ucg.snrcjt.cn

[R57] 远程执行命令
来源：http://whl.fktsv.cn

ssh user@host 'uptime'
来源：http://ljj.jqgfzy.top

[R58] 下载文件
来源：http://zhl.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://msj.yj20258.top

[R59] 发 POST JSON
来源：http://xki.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kuc.yfazqb.com

[R60] 只看 HTTP 状态码
来源：http://abq.fengsongda.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dfx.yuanzhike.top

[R61] 磁盘占用
来源：http://jws.yvedp.cn

df -h;  du -sh *
来源：http://eun.cqqwz.cn

[R62] 找最占空间的文件
来源：http://cvc.zhiwuduotai.top

du -ah . | sort -rh | head -10
来源：http://ecv.xuanzx.com

[R63] 内存与进程
来源：http://iyd.hammf.cn

free -h;  ps aux | grep nginx
来源：http://wqo.hesvh.cn

[R64] 结束进程
来源：http://btk.fanxiaobao.xyz

kill -9 $(pgrep -f app.py)
来源：http://gez.zdbjq.cn

[R65] 查看端口占用
来源：http://zst.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eqm.hysaishi.cn

[R66] 定时任务
来源：http://dnb.smart0.xyz

crontab -e;  crontab -l
来源：http://zvx.redwolf501.top

[R67] 生成随机十六进制串
来源：http://cgj.fanxiaobao.xyz

openssl rand -hex 16
来源：http://jnv.zhoulong.xyz

[R68] 计算文件校验值
来源：http://iir.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://qgg.cqqwz.cn

[R69] 生成随机密码
来源：http://xxh.shuidangran.top

head -c 16 /dev/urandom | base64
来源：http://hvp.tanke756.top

[R70] 时间戳与互转
来源：http://erg.sweek.top

date +%s;  date -d @1700000000
来源：http://wdp.yvedp.cn

[R71] 日期格式化
来源：http://mho.dianchejie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uei.cdnleiting.top

[R72] 等待端口就绪
来源：http://bvm.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uta.yuanzhike.top

[R73] 分割大日志
来源：http://xyn.jianghu66.top

split -l 1000 big.log part_
来源：http://plm.jinghuilouyu.cn

[R74] 批量重命名
来源：http://dyw.fehbvm.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lsd.guannengcc.top

[R75] 导出环境变量
来源：http://idm.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://nzm.hcnkem.com

[R76] 使用临时文件
来源：http://npi.svipenyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ijt.316326.xyz

[R77] 读取用户输入
来源：http://ogd.bjfxy.top

read -rp "请输入: " ans
来源：http://imi.zhiwuduotai.top

[R78] 交互式菜单
来源：http://elf.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://naj.yfazqb.com

[R79] 解析命令行选项
来源：http://ssp.jqgfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fqw.hnqzz.top

[R80] 查看脚本执行耗时
来源：http://nqb.zhoulong.xyz

time ./run.sh
来源：http://zdj.jqgfzy.top

================================================================================
来源：http://mgn.xingfuxueyuan.xyz

S. C / C++ 专题
来源：http://lby.chenzaomai.com

================================================================================
来源：http://sjb.nanxuanxn.top

[S01] C：Hello World
来源：http://jgr.sxryk.cn

#include <stdio.h>
来源：http://mom.fehbvm.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://yif.daria6918.cn

[S02] C：变量与格式化输出
来源：http://wsf.fengsongda.top

int a = 10; printf("%d\n", a);
来源：http://jov.yvedp.cn

[S03] C：读入整数
来源：http://uhb.uphjek.com

int x; scanf("%d", &x);
来源：http://bxv.jinqigufen.top

[S04] C：字符串复制
来源：http://sem.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://osg.shzxlz.cn

[S05] C：字符串长度
来源：http://xie.vqdsnc.cn

strlen(s)
来源：http://hmb.feifeiyinyue.top

[S06] C：字符串比较
来源：http://kxp.cheryme.top

strcmp(a, b) == 0
来源：http://txl.wangshuangyany.cn

[S07] C：数组遍历求和
来源：http://srg.xuanzx.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dws.dashuyun.cn

[S08] C：动态内存分配与释放
来源：http://pfm.0kj1m.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bgb.vqdsnc.cn

[S09] C：结构体定义与初始化
来源：http://qhu.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ery.daxiang520.top

[S10] C：指针与解引用
来源：http://swt.xingfuxueyuan.xyz

int *p = &a;  *p = 5;
来源：http://ysb.xylfe.cn

[S11] C：逐行读文件
来源：http://rao.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://pzy.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ymq.hcnkem.com

fclose(f);
来源：http://tei.yuxming.cn

[S12] C：写文件
来源：http://qif.yj202588.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lni.wangshuangyany.cn

[S13] C：宏定义
来源：http://opb.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yyr.bjfxy.top

[S14] C：枚举
来源：http://bju.hysaishi.cn

enum Color { RED, GREEN, BLUE };
来源：http://zsf.cucudq.cn

[S15] C：类型转换
来源：http://czp.iojbl.cn

(double) a / b
来源：http://afv.ppjwa.cn

[S16] C：位操作置位
来源：http://tde.uphjek.com

x |= (1 << 3);
来源：http://nby.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://kaw.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://swy.ctjpmb.com

[S18] C：命令行参数
来源：http://aml.tianlin.xyz

int main(int argc, char **argv)
来源：http://zhn.zhengqikj.top

[S19] C：快速排序
来源：http://ywk.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://xdd.shanyushiyangkeji.top

[S20] C：二分查找
来源：http://wzz.zhijiandao.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://idm.cheryme.top

[S21] C：字符类别判断
来源：http://sgk.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://enq.uphjek.com

[S22] C：字符串转数字
来源：http://jei.iojbl.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hno.ydzc1.top

[S23] C：随机数
来源：http://cgn.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://urp.ybcxt.top

[S24] C：获取本地时间
来源：http://ang.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tap.hammf.cn

[S25] C：内存拷贝
来源：http://jbc.ehwqpu.com

memcpy(dst, src, n);
来源：http://lpp.hcnkem.com

[S26] C：内存清零
来源：http://uch.fehbvm.com

memset(a, 0, sizeof a);
来源：http://fxd.yuanzhike.top

[S27] C：定义常量
来源：http://xhe.yvedp.cn

const double PI = 3.14159;
来源：http://jnu.nanxinkj.top

[S28] C：静态变量
来源：http://jvz.sjlbkw.cn

static int counter = 0;
来源：http://ixk.zhengqikj.top

[S29] C：变参函数
来源：http://sfl.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wyb.zhoulong.xyz

[S30] C：头文件保护
来源：http://vgh.dashuyun.cn

#ifndef X_H
来源：http://jgx.ybcxt.top

#define X_H
来源：http://olx.nwbrower.top

#endif
来源：http://rjg.andypj.xyz

[S31] C++：Hello World
来源：http://uvy.yangfankeji.com

#include <iostream>
来源：http://wea.yuanzhike.top

int main() { std::cout << "Hello\n"; }
来源：http://wvq.yj202588.top

[S32] C++：字符串
来源：http://ccp.ywan-chungtsiang.top

std::string s = "hi";  s += "!";
来源：http://bvj.tanke756.top

[S33] C++：vector 增删
来源：http://cfs.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oai.ivvv.top

[S34] C++：遍历 vector
来源：http://qfc.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://oqs.yueranfly.top

[S35] C++：map
来源：http://abw.jinqigufen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yuq.kuanghao11.cn

[S36] C++：unordered_map
来源：http://lbb.havefunace.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rxo.cheryme.top

[S37] C++：set
来源：http://wgq.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://snv.shanyushiyangkeji.top

[S38] C++：排序
来源：http://phb.fanxiaobao.xyz

std::sort(v.begin(), v.end());
来源：http://mxm.cqqwz.cn

[S39] C++：自定义比较器排序
来源：http://wyb.andypj.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://auw.ehwqpu.com

[S40] C++：查找元素
来源：http://tvu.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yav.9152youxi.cn

[S41] C++：类与构造函数
来源：http://usf.fanxiaobao.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ody.birdmap.top

[S42] C++：继承与虚函数
来源：http://rrj.zhoulong.xyz

class B : public Base { public: void f() override {} };
来源：http://ilh.hesvh.cn

[S43] C++：智能指针
来源：http://byl.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://xwz.tarul.cn

[S44] C++：引用传参
来源：http://otz.sweek.top

void inc(int &x) { ++x; }
来源：http://hqw.hnqzz.top

[S45] C++：lambda
来源：http://nqs.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://kzr.gaohongyu789.top

[S46] C++：函数模板
来源：http://ktd.zdqjudy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pui.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://zxj.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dqn.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://fwy.jyoumei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://unb.sweek.top

while (std::getline(in, line)) { }
来源：http://jvg.cheryme.top

[S49] C++：写文件
来源：http://rhf.daria6918.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xkn.sweek.top

[S50] C++：格式化数字
来源：http://yuo.zhengqikj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nvm.cheryme.top

[S51] C++：显式类型转换
来源：http://fht.jinqigfzy.top

static_cast<double>(a) / b
来源：http://jbd.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://xwh.jinqigufen.top

int size() const noexcept { return n_; }
来源：http://upx.havefunace.top

[S53] C++：移动语义
来源：http://uay.jyoumei.cn

std::vector<int> w = std::move(v);
来源：http://ulg.hnqzz.top

[S54] C++：异常处理
来源：http://rax.9152youxi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rzr.yangfankeji.com

[S55] C++：结构化绑定
来源：http://drx.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://aqo.guannengcc.top

[S56] C++：optional
来源：http://cty.zhongyouzk.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vga.ivvv.top

[S57] C++：编译期常量
来源：http://des.fktsv.cn

constexpr int N = 10;
来源：http://src.jinqigfzy.top

[S58] C++：命名空间
来源：http://csh.tarul.cn

namespace ns { int f() { return 1; } }
来源：http://bhu.ywan-chungtsiang.top

[S59] C++：静态断言
来源：http://zqq.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nbr.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://wqo.yueranfly.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ljk.hfpthk.cn

================================================================================
来源：http://gss.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hiu.tianlin.xyz

================================================================================
来源：http://sov.fengsongda.top

[T01] Kotlin：Hello World
来源：http://wqt.yangfankeji.com

println("Hello")
来源：http://fye.dashuyun.cn

[T02] Kotlin：变量
来源：http://uhy.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kbw.ppjwa.cn

[T03] Kotlin：字符串模板
来源：http://yqe.dianchejie.cn

"值: $b"
来源：http://atz.zhongyouzk.top

[T04] Kotlin：空安全
来源：http://yup.tanke756.top

val n: String? = null;  n?.length
来源：http://zqe.fktsv.cn

[T05] Kotlin：when 表达式
来源：http://fqm.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nvt.ydjk.org.cn

[T06] Kotlin：集合映射
来源：http://imv.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://czk.ydjk.org.cn


<!-- 参考信息 -->