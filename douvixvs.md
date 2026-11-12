代发 wailian999

case "$1" in
来源：http://ash.cashguo.top

start) echo "启动" ;;
来源：http://lqi.redwolf501.top

stop)  echo "停止" ;;
来源：http://zdq.hesvh.cn

*)     echo "未知命令" ;;
来源：http://eph.quarkkingdee.top

esac
来源：http://xoq.cucudq.cn

[R12] for 遍历文件
来源：http://wzf.zhengqikj.top

for f in *.txt; do echo "$f"; done
来源：http://zej.vqdsnc.cn

[R13] for 计数循环
来源：http://rbc.hysaishi.cn

for i in {1..10}; do echo "$i"; done
来源：http://tjv.gogol.net.cn

[R14] C 风格 for
来源：http://gnm.gotoacloud.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://npf.tian-w.cn

[R15] while 逐行读文件
来源：http://joo.guowangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ays.cdnleiting.top

[R16] until 等待条件
来源：http://twj.hysaishi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uvt.jiagoushi.top

[R17] 数组定义与取值
来源：http://jhh.tarul.cn

arr=(a b c); echo "${arr[0]}"
来源：http://iii.gaohongyu789.top

[R18] 遍历数组
来源：http://rns.jinyuanbaomall.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gns.iojbl.cn

[R19] 数组长度
来源：http://fhr.ydzc1.top

echo "${#arr[@]}"
来源：http://rdp.hammf.cn

[R20] 关联数组（字典）
来源：http://szc.cashguo.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bnk.ppjwa.cn

[R21] 字符串长度
来源：http://rmp.aizwys.cn

echo "${#s}"
来源：http://yvg.epnwcf.com

[R22] 截取子串
来源：http://uew.daxiang520.top

echo "${s:0:5}"
来源：http://vyl.yueranfly.top

[R23] 字符串替换
来源：http://bke.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kce.yonumen.top

[R24] 大小写转换
来源：http://fnv.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://gio.zhoulong.xyz

[R25] 去后缀 / 去前缀
来源：http://xlm.52xcode.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lmg.jlsjyb.cn

[R26] 命令替换
来源：http://jgv.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://njc.dashuyun.cn

[R27] 算术展开
来源：http://pxi.cashguo.top

echo $((1 + 2 * 3))
来源：http://ajd.sysykeji.top

[R28] 浮点运算
来源：http://qnw.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://jxr.fzhhl.top

[R29] 定义函数
来源：http://bin.bjfxy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mgp.guowangkeji.top

[R30] 函数返回状态码
来源：http://dti.ivvv.top

f() { return 0; }; f || echo "失败了"
来源：http://trr.gogol.net.cn

[R31] 局部变量
来源：http://lhu.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://tmo.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://wqp.jinqigfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://urz.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://gdt.yangfankeji.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://npn.fktsv.cn

[R34] 退出时清理
来源：http://xyr.tarul.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xnv.yuanzhike.top

[R35] 后台执行并等待
来源：http://zrj.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hkj.yueranfly.top

[R36] 并发执行多个任务
来源：http://cfx.zdbjq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oiv.52xcode.cn

[R37] 把输出赋给变量
来源：http://nhr.316326.xyz

files=$(ls -1)
来源：http://lhg.guowangkeji.top

[R38] 管道串联
来源：http://vhv.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://nvx.hammf.cn

[R39] 重定向标准输出与错误
来源：http://asz.daxiang520.top

cmd > out.log 2>&1
来源：http://cds.sjlbkw.cn

[R40] 追加写日志
来源：http://icz.snrcjt.cn

echo "log" >> out.log
来源：http://cbw.yongpay.top

[R41] 丢弃输出
来源：http://kjq.epnwcf.com

cmd >/dev/null 2>&1
来源：http://koq.316326.xyz

[R42] 输入重定向
来源：http://ozp.52xcode.cn

wc -l < a.txt
来源：http://dqr.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://ics.tianlin.xyz

find . -name "*.log" -type f
来源：http://jft.zhoulong.xyz

[R44] 按修改时间查找
来源：http://soq.jiagoushi.top

find . -mtime -7 -type f
来源：http://cwl.redwolf501.top

[R45] 批量删除
来源：http://erg.yonumen.top

find . -name "*.tmp" -delete
来源：http://wsp.hesvh.cn

[R46] 递归替换文件内容
来源：http://gzb.guannengcc.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ycf.tian-w.cn

[R47] sed 单行替换
来源：http://cvj.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tdh.hammf.cn

[R48] awk 取指定列
来源：http://yfw.fzhhl.top

awk '{print $1, $3}' a.txt
来源：http://pcd.fehbvm.com

[R49] awk 带条件
来源：http://nkg.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sly.shangyingyoupin.top

[R50] awk 求和
来源：http://uts.xziqi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rum.gzhubu.top

[R51] 排序去重取前几
来源：http://pbq.guowangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://erf.chenjidiqi.icu

[R52] 统计行数
来源：http://ztg.cheryme.top

wc -l a.txt
来源：http://mro.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://vgm.quarkkingdee.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nlm.wangdashe.top

[R54] 比较两个文件
来源：http://lrm.jqgfzy.top

diff a.txt b.txt
来源：http://ydl.9152youxi.cn

[R55] 压缩与解压
来源：http://prf.epnwcf.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sgn.shzxlz.cn

[R56] 远程拷贝
来源：http://tvc.smart0.xyz

scp file user@host:/path/
来源：http://ubj.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://kzm.jinqigfzy.top

ssh user@host 'uptime'
来源：http://wit.jyoumei.cn

[R58] 下载文件
来源：http://hac.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xlc.hcnkem.com

[R59] 发 POST JSON
来源：http://wyf.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ozf.tanke756.top

[R60] 只看 HTTP 状态码
来源：http://fwz.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hbn.andypj.xyz

[R61] 磁盘占用
来源：http://hqt.ydjk.org.cn

df -h;  du -sh *
来源：http://nak.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://vck.smart0.xyz

du -ah . | sort -rh | head -10
来源：http://fuc.gaohongyu789.top

[R63] 内存与进程
来源：http://yjz.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://gxl.zhoulong.xyz

[R64] 结束进程
来源：http://lte.yanxiufei.cn

kill -9 $(pgrep -f app.py)
来源：http://yay.jqgfzy.top

[R65] 查看端口占用
来源：http://ons.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pra.316326.xyz

[R66] 定时任务
来源：http://zmt.hnqzz.top

crontab -e;  crontab -l
来源：http://yed.kuanghao11.cn

[R67] 生成随机十六进制串
来源：http://jwe.yanxiufei.cn

openssl rand -hex 16
来源：http://dlj.hfpthk.cn

[R68] 计算文件校验值
来源：http://kny.gotoacloud.top

sha256sum a.txt;  md5sum a.txt
来源：http://wzs.sxryk.cn

[R69] 生成随机密码
来源：http://axw.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://scn.mhx1999.top

[R70] 时间戳与互转
来源：http://xqe.vehdjk.com

date +%s;  date -d @1700000000
来源：http://wrr.xingfuxueyuan.xyz

[R71] 日期格式化
来源：http://mri.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dxa.aizwys.cn

[R72] 等待端口就绪
来源：http://xiy.shuidangran.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jdy.jqgfzy.top

[R73] 分割大日志
来源：http://okz.yj202588.top

split -l 1000 big.log part_
来源：http://rch.jinqigufen.top

[R74] 批量重命名
来源：http://pkq.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pcn.daxiang520.top

[R75] 导出环境变量
来源：http://jxi.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://gbz.bjfxy.top

[R76] 使用临时文件
来源：http://afx.9152youxi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cvx.nanxinkj.top

[R77] 读取用户输入
来源：http://lrm.sjlbkw.cn

read -rp "请输入: " ans
来源：http://lxa.hywenlv.cn

[R78] 交互式菜单
来源：http://bfg.zhongyouzk.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xkg.dianchejie.cn

[R79] 解析命令行选项
来源：http://qth.zhoulong.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mrf.wangdashe.top

[R80] 查看脚本执行耗时
来源：http://knq.cqqwz.cn

time ./run.sh
来源：http://bvk.zhengqikj.top

================================================================================
来源：http://cgw.smart0.xyz

S. C / C++ 专题
来源：http://qen.pycfn.com

================================================================================
来源：http://syb.xinyue.icu

[S01] C：Hello World
来源：http://pjn.ybcxt.top

#include <stdio.h>
来源：http://nuo.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://olo.ywan-chungtsiang.top

[S02] C：变量与格式化输出
来源：http://npv.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://hvb.fehbvm.com

[S03] C：读入整数
来源：http://eun.ybcxt.top

int x; scanf("%d", &x);
来源：http://kgo.vehdjk.com

[S04] C：字符串复制
来源：http://sxu.jinqigufen.top

char dst[32]; strcpy(dst, "hi");
来源：http://aae.cashguo.top

[S05] C：字符串长度
来源：http://vcv.hnxiangtu.top

strlen(s)
来源：http://etn.tian-w.cn

[S06] C：字符串比较
来源：http://egs.chenlongwang.top

strcmp(a, b) == 0
来源：http://slo.ivvv.top

[S07] C：数组遍历求和
来源：http://rri.tarul.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xte.hammf.cn

[S08] C：动态内存分配与释放
来源：http://vui.zdqjudy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wfd.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://skh.svipenyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ozf.chenzaomai.com

[S10] C：指针与解引用
来源：http://fmf.hesvh.cn

int *p = &a;  *p = 5;
来源：http://qub.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://tcb.hfpthk.cn

FILE *f = fopen("a.txt", "r");
来源：http://cor.yj20258888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://aua.ctjpmb.com

fclose(f);
来源：http://hdj.zdqjudy.top

[S12] C：写文件
来源：http://ltv.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rlr.cashguo.top

[S13] C：宏定义
来源：http://ykl.52xcode.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lsv.gzhubu.top

[S14] C：枚举
来源：http://tzb.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://qwn.shuidangran.top

[S15] C：类型转换
来源：http://ujl.andypj.xyz

(double) a / b
来源：http://tdr.birdmap.top

[S16] C：位操作置位
来源：http://qih.bbcook.cn

x |= (1 << 3);
来源：http://bnp.hnxiangtu.top

[S17] C：安全拼接字符串
来源：http://toz.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://paq.nwbrower.top

[S18] C：命令行参数
来源：http://uma.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://kpo.chenjidiqi.icu

[S19] C：快速排序
来源：http://qkl.sweek.top

qsort(a, n, sizeof(int), cmp);
来源：http://tce.yfazqb.com

[S20] C：二分查找
来源：http://wos.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://owy.zdbjq.cn

[S21] C：字符类别判断
来源：http://mfm.gogol.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hvq.sweek.top

[S22] C：字符串转数字
来源：http://yxt.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://prj.yj20258888.top

[S23] C：随机数
来源：http://kaa.feifeiyinyue.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cgi.yanxiufei.cn

[S24] C：获取本地时间
来源：http://ibg.zycfv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oiy.daria6918.cn

[S25] C：内存拷贝
来源：http://rxg.zhixingplan.top

memcpy(dst, src, n);
来源：http://imm.tarul.cn

[S26] C：内存清零
来源：http://hdp.yuxming.cn

memset(a, 0, sizeof a);
来源：http://owh.jqgfzy.top

[S27] C：定义常量
来源：http://vjv.cheryme.top

const double PI = 3.14159;
来源：http://nfr.dashuyun.cn

[S28] C：静态变量
来源：http://xlc.chenjidiqi.icu

static int counter = 0;
来源：http://nsh.pengpengdd.cyou

[S29] C：变参函数
来源：http://szk.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://puu.jinyuanbaomall.cn

[S30] C：头文件保护
来源：http://dzj.yueranfly.top

#ifndef X_H
来源：http://axn.xuanzx.com

#define X_H
来源：http://gst.ydzc1.top

#endif
来源：http://iah.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://fni.yongpay.top

#include <iostream>
来源：http://nxu.gaohongyu789.top

int main() { std::cout << "Hello\n"; }
来源：http://kue.chenjidiqi.icu

[S32] C++：字符串
来源：http://gvi.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://xpa.yfazqb.com

[S33] C++：vector 增删
来源：http://ayh.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://opw.zhixingplan.top

[S34] C++：遍历 vector
来源：http://iuv.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://bum.tian-w.cn

[S35] C++：map
来源：http://znx.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vyl.fktsv.cn

[S36] C++：unordered_map
来源：http://mvh.mhx1999.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lnp.nanxinkj.top

[S37] C++：set
来源：http://ddi.meibo888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fid.gaohongyu789.top

[S38] C++：排序
来源：http://mbd.tarul.cn

std::sort(v.begin(), v.end());
来源：http://ksa.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://crb.yj20258.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dzr.birdmap.top

[S40] C++：查找元素
来源：http://knz.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pwr.yfazqb.com

[S41] C++：类与构造函数
来源：http://ptw.0kj1m.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dka.zycfv.cn

[S42] C++：继承与虚函数
来源：http://frt.wangdashe.top

class B : public Base { public: void f() override {} };
来源：http://nck.0kj1m.cn

[S43] C++：智能指针
来源：http://wua.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://nys.yongpay.top

[S44] C++：引用传参
来源：http://ywv.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://tbp.chenlongwang.top

[S45] C++：lambda
来源：http://ujl.nwbrower.top

auto add = [](int a, int b) { return a + b; };
来源：http://tyg.chenjidiqi.icu

[S46] C++：函数模板
来源：http://vud.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mbx.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://qns.kuanghao11.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aes.fengsongda.top

[S48] C++：逐行读文件
来源：http://bwi.hesvh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xel.yangfankeji.com

while (std::getline(in, line)) { }
来源：http://asz.yj20258888.top

[S49] C++：写文件
来源：http://jci.xylfe.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jyl.aizwys.cn

[S50] C++：格式化数字
来源：http://jqp.snrcjt.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ptc.chenzaomai.com

[S51] C++：显式类型转换
来源：http://mww.chenlongwang.top

static_cast<double>(a) / b
来源：http://oam.c1oappe.top

[S52] C++：const 与 noexcept
来源：http://hhi.sweek.top

int size() const noexcept { return n_; }
来源：http://bvv.jyoumei.cn

[S53] C++：移动语义
来源：http://sxl.bjfxy.top

std::vector<int> w = std::move(v);
来源：http://oug.yuxming.cn

[S54] C++：异常处理
来源：http://rrv.yangfankeji.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uba.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://rxz.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qzh.zdqjudy.top

[S56] C++：optional
来源：http://mii.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cal.ivvv.top

[S57] C++：编译期常量
来源：http://rav.xuanzx.com

constexpr int N = 10;
来源：http://zny.jyoumei.cn

[S58] C++：命名空间
来源：http://gav.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://ops.svipenyu.cn

[S59] C++：静态断言
来源：http://vnn.ehwqpu.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://swb.tian-w.cn

[S60] C++：遍历并删除元素
来源：http://lzf.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://snv.xylfe.cn

================================================================================
来源：http://ivi.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://afu.hnqzz.top

================================================================================
来源：http://imk.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://rem.jinyuanbaomall.cn

println("Hello")
来源：http://gze.52xcode.cn

[T02] Kotlin：变量
来源：http://vhr.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sfi.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://ezj.jqgfzy.top

"值: $b"
来源：http://wbd.tarul.cn

[T04] Kotlin：空安全
来源：http://chg.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://txy.sjlbkw.cn

[T05] Kotlin：when 表达式
来源：http://eot.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tcq.ydzc1.top

[T06] Kotlin：集合映射
来源：http://lib.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://sbp.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://aek.jinqigufen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ers.chenzaomai.com

[T08] Kotlin：数据类
来源：http://llc.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://ffp.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://kmw.aibaodan.cn

fun String.exclaim() = this + "!"
来源：http://ldc.yuanzhike.top

[T10] Kotlin：默认参数
来源：http://xqg.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://azh.haohaochexian.top

[T11] Kotlin：协程
来源：http://pvk.cucudq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://riz.cdnleiting.top

[T12] Kotlin：解构声明
来源：http://ilq.hfpthk.cn

val (a, b) = Pair(1, 2)
来源：http://ypg.gogol.net.cn


<!-- 参考信息 -->