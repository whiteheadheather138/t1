代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pep.fengsongda.top

[R16] until 等待条件
来源：http://hdc.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eaz.jiagoushi.top

[R17] 数组定义与取值
来源：http://sjl.52xcode.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ibz.quarkkingdee.top

[R18] 遍历数组
来源：http://oeu.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zpo.jlsjyb.cn

[R19] 数组长度
来源：http://ciw.ywan-chungtsiang.top

echo "${#arr[@]}"
来源：http://etr.hesvh.cn

[R20] 关联数组（字典）
来源：http://lsp.iojbl.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://thf.52xcode.cn

[R21] 字符串长度
来源：http://uab.hesvh.cn

echo "${#s}"
来源：http://dxq.hcnkem.com

[R22] 截取子串
来源：http://wzl.zhixingplan.top

echo "${s:0:5}"
来源：http://rgv.wangshuangyany.cn

[R23] 字符串替换
来源：http://glm.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kpo.dashuyun.cn

[R24] 大小写转换
来源：http://kko.gaohongyu789.top

echo "${s^^}"; echo "${s,,}"
来源：http://hyc.yj20258888.top

[R25] 去后缀 / 去前缀
来源：http://tbs.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://rvd.zhixingplan.top

[R26] 命令替换
来源：http://hru.yj202588.top

now=$(date +%F); echo "$now"
来源：http://uam.nanxuanxn.top

[R27] 算术展开
来源：http://gkd.jlsjyb.cn

echo $((1 + 2 * 3))
来源：http://org.ehwqpu.com

[R28] 浮点运算
来源：http://nng.cucudq.cn

echo "scale=2; 10/3" | bc
来源：http://ysh.jyoumei.cn

[R29] 定义函数
来源：http://xmm.ywan-chungtsiang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fti.gaohongyu789.top

[R30] 函数返回状态码
来源：http://llh.wangdashe.top

f() { return 0; }; f || echo "失败了"
来源：http://rrv.daria6918.cn

[R31] 局部变量
来源：http://ovu.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://ess.chenlongwang.top

[R32] 参数个数校验
来源：http://xwi.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rjz.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://xkj.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yzk.yanxiufei.cn

[R34] 退出时清理
来源：http://xmc.quarkkingdee.top

trap 'rm -f "$tmp"' EXIT
来源：http://lds.9152youxi.cn

[R35] 后台执行并等待
来源：http://yvt.cucudq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kee.birdmap.top

[R36] 并发执行多个任务
来源：http://zdd.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jdz.shzxlz.cn

[R37] 把输出赋给变量
来源：http://gfv.wangdashe.top

files=$(ls -1)
来源：http://mhn.birdmap.top

[R38] 管道串联
来源：http://kwr.shanyushiyangtech.top

cat a.txt | grep -i error | wc -l
来源：http://uvc.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://hcb.xuanzx.com

cmd > out.log 2>&1
来源：http://vrf.c1oappe.top

[R40] 追加写日志
来源：http://eas.hfpthk.cn

echo "log" >> out.log
来源：http://xoy.hesvh.cn

[R41] 丢弃输出
来源：http://qjl.jiagoushi.top

cmd >/dev/null 2>&1
来源：http://mof.daria6918.cn

[R42] 输入重定向
来源：http://xsj.xuanzx.com

wc -l < a.txt
来源：http://uxg.nwbrower.top

[R43] 按名字查找文件
来源：http://cav.xylfe.cn

find . -name "*.log" -type f
来源：http://brj.yj202588.top

[R44] 按修改时间查找
来源：http://oop.cashguo.top

find . -mtime -7 -type f
来源：http://bvt.ivvv.top

[R45] 批量删除
来源：http://vys.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://pmq.bbcook.cn

[R46] 递归替换文件内容
来源：http://dip.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yro.havefunace.top

[R47] sed 单行替换
来源：http://asm.aizwys.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hrj.yanxiufei.cn

[R48] awk 取指定列
来源：http://udi.aibaodan.cn

awk '{print $1, $3}' a.txt
来源：http://laf.fktsv.cn

[R49] awk 带条件
来源：http://azu.shanyushiyangtech.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fvm.yongpay.top

[R50] awk 求和
来源：http://vha.cashguo.top

awk '{s += $2} END {print s}' a.txt
来源：http://ccz.yuanzhike.top

[R51] 排序去重取前几
来源：http://cce.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uys.yongpay.top

[R52] 统计行数
来源：http://sdg.snrcjt.cn

wc -l a.txt
来源：http://qnx.cheryme.top

[R53] 查看文件头与实时尾
来源：http://cds.jqgfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wtj.fzhhl.top

[R54] 比较两个文件
来源：http://jef.vehdjk.com

diff a.txt b.txt
来源：http://bxg.bjfxy.top

[R55] 压缩与解压
来源：http://jng.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hhf.sxryk.cn

[R56] 远程拷贝
来源：http://veh.sysykeji.top

scp file user@host:/path/
来源：http://hnj.yuanzhike.top

[R57] 远程执行命令
来源：http://qrd.aizwys.cn

ssh user@host 'uptime'
来源：http://nhi.sxryk.cn

[R58] 下载文件
来源：http://lwz.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ekr.jlsjyb.cn

[R59] 发 POST JSON
来源：http://dxc.fanxiaobao.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lim.xuetiantiany.cn

[R60] 只看 HTTP 状态码
来源：http://ukn.aibaodan.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qbu.cucudq.cn

[R61] 磁盘占用
来源：http://evu.zhengqikj.top

df -h;  du -sh *
来源：http://bvs.quarkkingdee.top

[R62] 找最占空间的文件
来源：http://elz.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://gzy.ppjwa.cn

[R63] 内存与进程
来源：http://vax.0kj1m.cn

free -h;  ps aux | grep nginx
来源：http://rgg.ywan-chungtsiang.top

[R64] 结束进程
来源：http://iae.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://khu.bjfxy.top

[R65] 查看端口占用
来源：http://fap.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nsw.jinghuilouyu.cn

[R66] 定时任务
来源：http://stt.epnwcf.com

crontab -e;  crontab -l
来源：http://vmb.yongpay.top

[R67] 生成随机十六进制串
来源：http://yiz.hfpthk.cn

openssl rand -hex 16
来源：http://tor.hcnkem.com

[R68] 计算文件校验值
来源：http://yjo.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://shp.hcnkem.com

[R69] 生成随机密码
来源：http://dfs.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://ajr.sweek.top

[R70] 时间戳与互转
来源：http://gop.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://ljh.xingfuxueyuan.xyz

[R71] 日期格式化
来源：http://pno.jqgfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lfp.tanke756.top

[R72] 等待端口就绪
来源：http://utx.hnxiangtu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mbz.svipenyu.cn

[R73] 分割大日志
来源：http://zgw.bbcook.cn

split -l 1000 big.log part_
来源：http://sef.cdnleiting.top

[R74] 批量重命名
来源：http://mgc.svipenyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mfu.bbcook.cn

[R75] 导出环境变量
来源：http://wwz.jinqigfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://orj.havefunace.top

[R76] 使用临时文件
来源：http://lrv.smart0.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fbw.redwolf501.top

[R77] 读取用户输入
来源：http://fka.yanxiufei.cn

read -rp "请输入: " ans
来源：http://ckc.yuanzhike.top

[R78] 交互式菜单
来源：http://ssv.nwbrower.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vkh.sjlbkw.cn

[R79] 解析命令行选项
来源：http://qhb.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://amx.sysykeji.top

[R80] 查看脚本执行耗时
来源：http://rqz.jinyuanbaomall.cn

time ./run.sh
来源：http://jtd.cashguo.top

================================================================================
来源：http://iwj.jyoumei.cn

S. C / C++ 专题
来源：http://qre.jqgfzy.top

================================================================================
来源：http://tvz.wangshuangyany.cn

[S01] C：Hello World
来源：http://tnm.mhx1999.top

#include <stdio.h>
来源：http://csg.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nxj.shanyushiyangkeji.top

[S02] C：变量与格式化输出
来源：http://uwn.svipenyu.cn

int a = 10; printf("%d\n", a);
来源：http://oxc.yanxiufei.cn

[S03] C：读入整数
来源：http://yyl.cashguo.top

int x; scanf("%d", &x);
来源：http://rex.bbcook.cn

[S04] C：字符串复制
来源：http://uhf.tianlin.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://eph.jinqigfzy.top

[S05] C：字符串长度
来源：http://ulh.sweek.top

strlen(s)
来源：http://xfa.nanxuanxn.top

[S06] C：字符串比较
来源：http://fov.sxryk.cn

strcmp(a, b) == 0
来源：http://qqw.ehwqpu.com

[S07] C：数组遍历求和
来源：http://xer.hesvh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ceo.shzxlz.cn

[S08] C：动态内存分配与释放
来源：http://nzw.yfazqb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pqr.yj20258.top

[S09] C：结构体定义与初始化
来源：http://yyq.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dlh.birdmap.top

[S10] C：指针与解引用
来源：http://ecv.ybcxt.top

int *p = &a;  *p = 5;
来源：http://hdq.fengsongda.top

[S11] C：逐行读文件
来源：http://bvv.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://pii.fehbvm.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ndd.xinyue.icu

fclose(f);
来源：http://ujp.xingfuxueyuan.xyz

[S12] C：写文件
来源：http://szl.bjfxy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lwl.xziqi.cn

[S13] C：宏定义
来源：http://xdm.yfazqb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hqy.shangyingyoupin.top

[S14] C：枚举
来源：http://nag.nanxuanxn.top

enum Color { RED, GREEN, BLUE };
来源：http://mzn.cucudq.cn

[S15] C：类型转换
来源：http://geu.daxiang520.top

(double) a / b
来源：http://koi.zhengqikj.top

[S16] C：位操作置位
来源：http://yej.svipenyu.cn

x |= (1 << 3);
来源：http://lfi.fktsv.cn

[S17] C：安全拼接字符串
来源：http://qlf.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://scy.aizwys.cn

[S18] C：命令行参数
来源：http://jmy.ivvv.top

int main(int argc, char **argv)
来源：http://pnt.yuanzhike.top

[S19] C：快速排序
来源：http://igr.sjlbkw.cn

qsort(a, n, sizeof(int), cmp);
来源：http://auh.c1oappe.top

[S20] C：二分查找
来源：http://ffk.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eku.bbcook.cn

[S21] C：字符类别判断
来源：http://mpc.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mzv.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://mla.gotoacloud.top

atoi("42");  strtod("3.14", NULL);
来源：http://dyu.jianghu66.top

[S23] C：随机数
来源：http://emv.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://txo.zhoulong.xyz

[S24] C：获取本地时间
来源：http://dxd.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://via.hcnkem.com

[S25] C：内存拷贝
来源：http://cle.hcnkem.com

memcpy(dst, src, n);
来源：http://mfz.gzhubu.top

[S26] C：内存清零
来源：http://kqz.gogol.net.cn

memset(a, 0, sizeof a);
来源：http://izr.sxryk.cn

[S27] C：定义常量
来源：http://uzo.9152youxi.cn

const double PI = 3.14159;
来源：http://ape.jyoumei.cn

[S28] C：静态变量
来源：http://rsb.cashguo.top

static int counter = 0;
来源：http://bgr.yj202588.top

[S29] C：变参函数
来源：http://iel.0kj1m.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://huz.hysaishi.cn

[S30] C：头文件保护
来源：http://zox.jinyuanbaomall.cn

#ifndef X_H
来源：http://emm.yj202588.top

#define X_H
来源：http://dob.yuanzhike.top

#endif
来源：http://mhb.hnxiangtu.top

[S31] C++：Hello World
来源：http://nio.nwbrower.top

#include <iostream>
来源：http://ahh.hcnkem.com

int main() { std::cout << "Hello\n"; }
来源：http://ird.xylfe.cn

[S32] C++：字符串
来源：http://ekx.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://gsg.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://gwg.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bot.xylfe.cn

[S34] C++：遍历 vector
来源：http://tno.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://dol.nanxinkj.top

[S35] C++：map
来源：http://nxn.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rky.yj202588.top

[S36] C++：unordered_map
来源：http://nbn.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gii.gogol.net.cn

[S37] C++：set
来源：http://vqh.hnqzz.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lzf.jyoumei.cn

[S38] C++：排序
来源：http://muz.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://zhh.vehdjk.com

[S39] C++：自定义比较器排序
来源：http://abd.hcnkem.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://shx.dianchejie.cn

[S40] C++：查找元素
来源：http://sep.zhongyouzk.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sxe.dashuyun.cn

[S41] C++：类与构造函数
来源：http://iqo.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rfd.gzhubu.top

[S42] C++：继承与虚函数
来源：http://eew.snrcjt.cn

class B : public Base { public: void f() override {} };
来源：http://pkp.ivvv.top

[S43] C++：智能指针
来源：http://xcx.fanxiaobao.xyz

auto p = std::make_unique<int>(5);
来源：http://quc.yj202588.top

[S44] C++：引用传参
来源：http://nzj.wangdashe.top

void inc(int &x) { ++x; }
来源：http://xys.quarkkingdee.top

[S45] C++：lambda
来源：http://sfh.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://nro.chenlongwang.top

[S46] C++：函数模板
来源：http://zqc.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sgv.pycfn.com

[S47] C++：结构化绑定遍历
来源：http://jor.snrcjt.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gkt.tian-w.cn

[S48] C++：逐行读文件
来源：http://eun.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://xzr.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://syp.jianghu66.top

[S49] C++：写文件
来源：http://zie.tarul.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cca.yj20258.top

[S50] C++：格式化数字
来源：http://atv.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hsy.daria6918.cn

[S51] C++：显式类型转换
来源：http://moe.shanyushiyangtech.top

static_cast<double>(a) / b
来源：http://gbh.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://kxf.ivvv.top

int size() const noexcept { return n_; }
来源：http://hhc.jyoumei.cn

[S53] C++：移动语义
来源：http://fgx.cheryme.top

std::vector<int> w = std::move(v);
来源：http://ajv.zdbjq.cn

[S54] C++：异常处理
来源：http://qrd.yj202588.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jrb.shanyushiyangkeji.top

[S55] C++：结构化绑定
来源：http://nul.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jjj.ywan-chungtsiang.top

[S56] C++：optional
来源：http://uwg.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wvw.hnqzz.top

[S57] C++：编译期常量
来源：http://qoy.jyoumei.cn

constexpr int N = 10;
来源：http://zsg.uphjek.com

[S58] C++：命名空间
来源：http://jcn.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://vei.hysaishi.cn

[S59] C++：静态断言
来源：http://fyi.zhengqikj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ksl.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://art.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fam.zdbjq.cn

================================================================================
来源：http://hkz.hysaishi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nke.zhoulong.xyz

================================================================================
来源：http://dnp.sweek.top

[T01] Kotlin：Hello World
来源：http://jxt.dianchejie.cn

println("Hello")
来源：http://cau.sxryk.cn

[T02] Kotlin：变量
来源：http://bhh.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ygm.bjfxy.top

[T03] Kotlin：字符串模板
来源：http://hsq.xylfe.cn

"值: $b"
来源：http://ilb.mhx1999.top

[T04] Kotlin：空安全
来源：http://gqw.haohaochexian.top

val n: String? = null;  n?.length
来源：http://gba.zhiwuduotai.top

[T05] Kotlin：when 表达式
来源：http://lsr.vehdjk.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://acu.vqdsnc.cn

[T06] Kotlin：集合映射
来源：http://xuf.gaohongyu789.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zcr.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://hli.hnxiangtu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://thp.nanxuanxn.top

[T08] Kotlin：数据类
来源：http://lrc.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://zke.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://lou.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://smz.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://thh.bjfxy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ptf.sweek.top

[T11] Kotlin：协程
来源：http://hfg.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ccr.nwbrower.top

[T12] Kotlin：解构声明
来源：http://vql.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://usc.epnwcf.com

[T13] Kotlin：只读 Map
来源：http://thi.yj20258.top

val m = mapOf("a" to 1)
来源：http://dbu.yongpay.top

[T14] Kotlin：循环
来源：http://zwl.fengsongda.top

for (i in 1..10) println(i)
来源：http://eex.cqqwz.cn

[T15] Kotlin：接口
来源：http://dua.nwbrower.top

interface Shape { fun area(): Double }
来源：http://wif.fengsongda.top

[T16] Swift：Hello World
来源：http://ghx.daria6918.cn

print("Hello")
来源：http://ojm.zhengqikj.top

[T17] Swift：变量与常量
来源：http://ipu.svipenyu.cn

var a = 1;  let b = 2
来源：http://jpu.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://nfy.sxryk.cn

"值: \(b)"
来源：http://yay.hywenlv.cn


<!-- 参考信息 -->