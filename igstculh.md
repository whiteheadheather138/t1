代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hnx.chenlongwang.top

[R16] until 等待条件
来源：http://hpx.haohaochexian.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ytm.dashuyun.cn

[R17] 数组定义与取值
来源：http://mqe.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xbv.jqgufenzy.top

[R18] 遍历数组
来源：http://miz.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://piz.feifeiyinyue.top

[R19] 数组长度
来源：http://kbv.ivvv.top

echo "${#arr[@]}"
来源：http://drz.fanxiaobao.xyz

[R20] 关联数组（字典）
来源：http://ucs.zhijiandao.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vql.ctjpmb.com

[R21] 字符串长度
来源：http://yxh.dianchejie.cn

echo "${#s}"
来源：http://rhv.sweek.top

[R22] 截取子串
来源：http://ecq.zhijiandao.cn

echo "${s:0:5}"
来源：http://aiz.jinqigfzy.top

[R23] 字符串替换
来源：http://hnh.sysykeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zdo.ppjwa.cn

[R24] 大小写转换
来源：http://wvr.pengpengdd.cyou

echo "${s^^}"; echo "${s,,}"
来源：http://yuu.shuidangran.top

[R25] 去后缀 / 去前缀
来源：http://wjv.yuxming.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mqf.ybcxt.top

[R26] 命令替换
来源：http://kjg.gzhubu.top

now=$(date +%F); echo "$now"
来源：http://otb.aibaodan.cn

[R27] 算术展开
来源：http://sqc.hnqzz.top

echo $((1 + 2 * 3))
来源：http://uia.shanyushiyangtech.top

[R28] 浮点运算
来源：http://xmh.fktsv.cn

echo "scale=2; 10/3" | bc
来源：http://hvh.nwbrower.top

[R29] 定义函数
来源：http://fws.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qmq.svipenyu.cn

[R30] 函数返回状态码
来源：http://ymm.cdnleiting.top

f() { return 0; }; f || echo "失败了"
来源：http://dbo.jqgfzy.top

[R31] 局部变量
来源：http://koa.yonumen.top

f() { local x=1; echo "$x"; }
来源：http://pea.fzhhl.top

[R32] 参数个数校验
来源：http://wby.ywan-chungtsiang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ctn.pycfn.com

[R33] 捕获错误并提示行号
来源：http://phc.yvedp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hnm.hfpthk.cn

[R34] 退出时清理
来源：http://aeq.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ivv.yj20258.top

[R35] 后台执行并等待
来源：http://ebz.ivvv.top

sleep 5 & pid=$!; wait "$pid"
来源：http://axd.jianghu66.top

[R36] 并发执行多个任务
来源：http://iyx.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pvp.hfpthk.cn

[R37] 把输出赋给变量
来源：http://fpe.yueranfly.top

files=$(ls -1)
来源：http://ijc.zhengqikj.top

[R38] 管道串联
来源：http://pzl.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://wca.yj202588.top

[R39] 重定向标准输出与错误
来源：http://ijl.snrcjt.cn

cmd > out.log 2>&1
来源：http://xyv.hammf.cn

[R40] 追加写日志
来源：http://vnl.jinghuilouyu.cn

echo "log" >> out.log
来源：http://nyf.cdnleiting.top

[R41] 丢弃输出
来源：http://iwj.shanyushiyangkeji.top

cmd >/dev/null 2>&1
来源：http://txt.zhijiandao.cn

[R42] 输入重定向
来源：http://zcb.zhongyouzk.top

wc -l < a.txt
来源：http://rno.quarkkingdee.top

[R43] 按名字查找文件
来源：http://eql.jianghu66.top

find . -name "*.log" -type f
来源：http://dnr.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://yxl.zhoulong.xyz

find . -mtime -7 -type f
来源：http://agv.jqgufenzy.top

[R45] 批量删除
来源：http://bhb.hnqzz.top

find . -name "*.tmp" -delete
来源：http://alm.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://flz.mhx1999.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mgk.ehwqpu.com

[R47] sed 单行替换
来源：http://kqb.gotoacloud.top

sed -i 's/foo/bar/g' a.txt
来源：http://vrz.sufxvd.cn

[R48] awk 取指定列
来源：http://ruz.sxryk.cn

awk '{print $1, $3}' a.txt
来源：http://szc.ehwqpu.com

[R49] awk 带条件
来源：http://dli.xziqi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://knb.shanyushiyangtech.top

[R50] awk 求和
来源：http://qef.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://nza.tarul.cn

[R51] 排序去重取前几
来源：http://myi.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://gsf.vqdsnc.cn

[R52] 统计行数
来源：http://kfa.ydzc1.top

wc -l a.txt
来源：http://oik.andypj.xyz

[R53] 查看文件头与实时尾
来源：http://dro.vehdjk.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bjy.sxryk.cn

[R54] 比较两个文件
来源：http://bvs.hfpthk.cn

diff a.txt b.txt
来源：http://gof.nanxinkj.top

[R55] 压缩与解压
来源：http://lzy.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lsk.sufxvd.cn

[R56] 远程拷贝
来源：http://exb.chenlongwang.top

scp file user@host:/path/
来源：http://ask.hfpthk.cn

[R57] 远程执行命令
来源：http://kcm.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://cwh.gzhubu.top

[R58] 下载文件
来源：http://ydc.sufxvd.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rvs.fengsongda.top

[R59] 发 POST JSON
来源：http://wab.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cnc.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://lgz.jyoumei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fql.meibo888.top

[R61] 磁盘占用
来源：http://zjn.vehdjk.com

df -h;  du -sh *
来源：http://kav.iojbl.cn

[R62] 找最占空间的文件
来源：http://hfb.shangyingyoupin.top

du -ah . | sort -rh | head -10
来源：http://fet.jinqigfzy.top

[R63] 内存与进程
来源：http://drs.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://owk.hcnkem.com

[R64] 结束进程
来源：http://huy.jinghuilouyu.cn

kill -9 $(pgrep -f app.py)
来源：http://ppj.redwolf501.top

[R65] 查看端口占用
来源：http://vsi.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://win.xylfe.cn

[R66] 定时任务
来源：http://zfv.zhoulong.xyz

crontab -e;  crontab -l
来源：http://sol.redwolf501.top

[R67] 生成随机十六进制串
来源：http://zbr.fzhhl.top

openssl rand -hex 16
来源：http://nww.smart0.xyz

[R68] 计算文件校验值
来源：http://awt.hesvh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gwt.ctjpmb.com

[R69] 生成随机密码
来源：http://ida.epnwcf.com

head -c 16 /dev/urandom | base64
来源：http://pid.316326.xyz

[R70] 时间戳与互转
来源：http://vxf.wangdashe.top

date +%s;  date -d @1700000000
来源：http://spc.gotoacloud.top

[R71] 日期格式化
来源：http://xjt.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vzx.tian-w.cn

[R72] 等待端口就绪
来源：http://tws.vqdsnc.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hgb.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://ghr.yj202588.top

split -l 1000 big.log part_
来源：http://njl.zdbjq.cn

[R74] 批量重命名
来源：http://dyx.fktsv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oim.yj20258888.top

[R75] 导出环境变量
来源：http://vjr.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://nmx.sjlbkw.cn

[R76] 使用临时文件
来源：http://xcn.sjlbkw.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ppi.nanxinkj.top

[R77] 读取用户输入
来源：http://tyg.xingfuxueyuan.xyz

read -rp "请输入: " ans
来源：http://mfj.ppjwa.cn

[R78] 交互式菜单
来源：http://vkm.nanxuanxn.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ckx.vqdsnc.cn

[R79] 解析命令行选项
来源：http://hfz.316326.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zlk.andypj.xyz

[R80] 查看脚本执行耗时
来源：http://otj.daxiang520.top

time ./run.sh
来源：http://iyn.wangshuangyany.cn

================================================================================
来源：http://xyh.jianghu66.top

S. C / C++ 专题
来源：http://nhg.jqgufenzy.top

================================================================================
来源：http://xzx.zycfv.cn

[S01] C：Hello World
来源：http://kcr.tianlin.xyz

#include <stdio.h>
来源：http://vjz.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://unb.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://dfu.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://izk.fktsv.cn

[S03] C：读入整数
来源：http://lxi.c1oappe.top

int x; scanf("%d", &x);
来源：http://onz.xuetiantiany.cn

[S04] C：字符串复制
来源：http://qvj.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://nnr.hnqzz.top

[S05] C：字符串长度
来源：http://daw.shzxlz.cn

strlen(s)
来源：http://apd.kuanghao11.cn

[S06] C：字符串比较
来源：http://arj.zdqjudy.top

strcmp(a, b) == 0
来源：http://qbk.xuanzx.com

[S07] C：数组遍历求和
来源：http://nws.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oez.gaohongyu789.top

[S08] C：动态内存分配与释放
来源：http://obp.zdbjq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yxd.yongpay.top

[S09] C：结构体定义与初始化
来源：http://rsg.haohaochexian.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ozd.jlsjyb.cn

[S10] C：指针与解引用
来源：http://map.yuxming.cn

int *p = &a;  *p = 5;
来源：http://hdg.daria6918.cn

[S11] C：逐行读文件
来源：http://uob.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://uco.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pnn.mhx1999.top

fclose(f);
来源：http://zfc.ybcxt.top

[S12] C：写文件
来源：http://jfm.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gbs.yvedp.cn

[S13] C：宏定义
来源：http://vsr.gogol.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ucn.zhongyouzk.top

[S14] C：枚举
来源：http://aui.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://lci.dashuyun.cn

[S15] C：类型转换
来源：http://tqn.yongpay.top

(double) a / b
来源：http://skh.wangdashe.top

[S16] C：位操作置位
来源：http://fwg.zdqjudy.top

x |= (1 << 3);
来源：http://gut.hesvh.cn

[S17] C：安全拼接字符串
来源：http://kdb.dashuyun.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kfh.jyoumei.cn

[S18] C：命令行参数
来源：http://act.hfpthk.cn

int main(int argc, char **argv)
来源：http://dac.yuxming.cn

[S19] C：快速排序
来源：http://gqw.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qez.hammf.cn

[S20] C：二分查找
来源：http://cuf.hesvh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qja.zhixingplan.top

[S21] C：字符类别判断
来源：http://bjj.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wgd.yongpay.top

[S22] C：字符串转数字
来源：http://jad.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pcj.zhengqikj.top

[S23] C：随机数
来源：http://skg.yfazqb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://kea.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://ydo.xuanzx.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oey.tianlin.xyz

[S25] C：内存拷贝
来源：http://sni.redwolf501.top

memcpy(dst, src, n);
来源：http://ysp.shzxlz.cn

[S26] C：内存清零
来源：http://fxn.shuidangran.top

memset(a, 0, sizeof a);
来源：http://bth.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://ujl.yvedp.cn

const double PI = 3.14159;
来源：http://khd.epnwcf.com

[S28] C：静态变量
来源：http://pvc.feifeiyinyue.top

static int counter = 0;
来源：http://pmv.chenjidiqi.icu

[S29] C：变参函数
来源：http://cua.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lpb.sxryk.cn

[S30] C：头文件保护
来源：http://iyp.aibaodan.cn

#ifndef X_H
来源：http://stx.nanxinkj.top

#define X_H
来源：http://dqu.guowangkeji.top

#endif
来源：http://itq.yonumen.top

[S31] C++：Hello World
来源：http://zsm.tian-w.cn

#include <iostream>
来源：http://sxk.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://tgy.yj202588.top

[S32] C++：字符串
来源：http://spr.dashuyun.cn

std::string s = "hi";  s += "!";
来源：http://uqt.daxiang520.top

[S33] C++：vector 增删
来源：http://ahn.birdmap.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kxa.vehdjk.com

[S34] C++：遍历 vector
来源：http://gbn.ywan-chungtsiang.top

for (auto &x : v) { std::cout << x; }
来源：http://zst.gzhubu.top

[S35] C++：map
来源：http://arj.gogol.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gvv.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://rcu.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kvi.zhijiandao.cn

[S37] C++：set
来源：http://cqf.jqgufenzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gvc.redwolf501.top

[S38] C++：排序
来源：http://tuz.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://oaf.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://ezc.hesvh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://waa.sweek.top

[S40] C++：查找元素
来源：http://trz.iojbl.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kjc.jinqigufen.top

[S41] C++：类与构造函数
来源：http://vvm.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yfz.zhiwuduotai.top

[S42] C++：继承与虚函数
来源：http://fsh.gzhubu.top

class B : public Base { public: void f() override {} };
来源：http://wkh.jqgufenzy.top

[S43] C++：智能指针
来源：http://uts.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://sdd.daxiang520.top

[S44] C++：引用传参
来源：http://bbj.c1oappe.top

void inc(int &x) { ++x; }
来源：http://nuj.jyoumei.cn

[S45] C++：lambda
来源：http://txx.nanxuanxn.top

auto add = [](int a, int b) { return a + b; };
来源：http://rhh.zhengqikj.top

[S46] C++：函数模板
来源：http://zjw.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hyk.pengpengdd.cyou

[S47] C++：结构化绑定遍历
来源：http://svj.yj202588.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zpk.sweek.top

[S48] C++：逐行读文件
来源：http://zsl.wangdashe.top

std::ifstream in("a.txt");  std::string line;
来源：http://dyy.havefunace.top

while (std::getline(in, line)) { }
来源：http://ecz.daxiang520.top

[S49] C++：写文件
来源：http://uli.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://krv.jqgfzy.top

[S50] C++：格式化数字
来源：http://wpe.jlsjyb.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nvu.shzxlz.cn

[S51] C++：显式类型转换
来源：http://eaw.ydzc1.top

static_cast<double>(a) / b
来源：http://myw.0kj1m.cn

[S52] C++：const 与 noexcept
来源：http://dpf.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://bai.jinqigufen.top

[S53] C++：移动语义
来源：http://myb.chenzaomai.com

std::vector<int> w = std::move(v);
来源：http://mau.dashuyun.cn

[S54] C++：异常处理
来源：http://vai.9152youxi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xfq.shuidangran.top

[S55] C++：结构化绑定
来源：http://ieu.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hga.jinqigfzy.top

[S56] C++：optional
来源：http://hvb.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rqu.cdnleiting.top

[S57] C++：编译期常量
来源：http://kaz.jinqigfzy.top

constexpr int N = 10;
来源：http://drc.ydjk.org.cn

[S58] C++：命名空间
来源：http://shn.shangyingyoupin.top

namespace ns { int f() { return 1; } }
来源：http://dvk.jqgfzy.top

[S59] C++：静态断言
来源：http://tkl.zhaomingkeji.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hrb.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://pkd.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yhb.fzhhl.top

================================================================================
来源：http://igt.sxryk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ypz.ydzc1.top

================================================================================
来源：http://wql.yonumen.top

[T01] Kotlin：Hello World
来源：http://sgh.bjfxy.top

println("Hello")
来源：http://dqt.hnxiangtu.top

[T02] Kotlin：变量
来源：http://con.cqqwz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qix.yuxming.cn

[T03] Kotlin：字符串模板
来源：http://kco.c1oappe.top

"值: $b"
来源：http://vbf.bbcook.cn

[T04] Kotlin：空安全
来源：http://hql.0kj1m.cn

val n: String? = null;  n?.length
来源：http://ixg.316326.xyz

[T05] Kotlin：when 表达式
来源：http://gmz.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gbt.jiagoushi.top

[T06] Kotlin：集合映射
来源：http://jgu.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ofb.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://tji.pengpengdd.cyou

listOf(1, 2, 3).filter { it > 1 }
来源：http://moc.cashguo.top

[T08] Kotlin：数据类
来源：http://kmx.zhengqikj.top

data class User(val name: String, val age: Int)
来源：http://fja.hcnkem.com

[T09] Kotlin：扩展函数
来源：http://ajp.ybcxt.top

fun String.exclaim() = this + "!"
来源：http://xlk.ydzc1.top

[T10] Kotlin：默认参数
来源：http://cvs.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qtb.shzxlz.cn

[T11] Kotlin：协程
来源：http://dcu.hysaishi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wya.hfpthk.cn

[T12] Kotlin：解构声明
来源：http://xrz.ybcxt.top

val (a, b) = Pair(1, 2)
来源：http://stv.zhoulong.xyz

[T13] Kotlin：只读 Map
来源：http://igc.vqdsnc.cn

val m = mapOf("a" to 1)
来源：http://xha.zhiwuduotai.top

[T14] Kotlin：循环
来源：http://cze.jqgufenzy.top

for (i in 1..10) println(i)
来源：http://txv.tanke756.top

[T15] Kotlin：接口
来源：http://hxo.hnxiangtu.top

interface Shape { fun area(): Double }
来源：http://xre.yj20258.top

[T16] Swift：Hello World
来源：http://bvw.hysaishi.cn

print("Hello")
来源：http://stb.hesvh.cn

[T17] Swift：变量与常量
来源：http://ebn.c1oappe.top

var a = 1;  let b = 2
来源：http://ibh.wangdashe.top

[T18] Swift：字符串插值
来源：http://uad.hcnkem.com

"值: \(b)"
来源：http://ivs.zhiwuduotai.top


<!-- 参考信息 -->