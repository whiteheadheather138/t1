代发 wailian999

readonly PI=3.14
来源：http://vrh.jinghuilouyu.cn

[R04] 位置参数
来源：http://xcl.snrcjt.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qkw.ctjpmb.com

[R05] 参数默认值
来源：http://cdm.ppjwa.cn

name="${1:-default}"
来源：http://mce.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://fux.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kbj.vehdjk.com

[R07] if 判断文件
来源：http://pzr.0kj1m.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bpo.hesvh.cn

[R08] 数值比较
来源：http://sfb.nwbrower.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dvc.gogol.net.cn

[R09] 字符串比较
来源：http://tne.tarul.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bnb.yuxming.cn

[R10] 正则匹配
来源：http://osr.xylfe.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ejs.uphjek.com

[R11] case 多分支
来源：http://ekb.hongshengwenyu.top

case "$1" in
来源：http://rid.ctjpmb.com

start) echo "启动" ;;
来源：http://xuh.yj202588.top

stop)  echo "停止" ;;
来源：http://zsh.shuidangran.top

*)     echo "未知命令" ;;
来源：http://idt.snrcjt.cn

esac
来源：http://gkh.zycfv.cn

[R12] for 遍历文件
来源：http://tiy.mhx1999.top

for f in *.txt; do echo "$f"; done
来源：http://zxn.52xcode.cn

[R13] for 计数循环
来源：http://nzb.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://rie.sufxvd.cn

[R14] C 风格 for
来源：http://cus.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ijg.jinyuanbaomall.cn

[R15] while 逐行读文件
来源：http://gcx.dashuyun.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hus.yongpay.top

[R16] until 等待条件
来源：http://bvq.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dnj.cheryme.top

[R17] 数组定义与取值
来源：http://mth.52xcode.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cij.fehbvm.com

[R18] 遍历数组
来源：http://eaf.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lwj.shangyingyoupin.top

[R19] 数组长度
来源：http://hpr.guannengcc.top

echo "${#arr[@]}"
来源：http://wjr.yvedp.cn

[R20] 关联数组（字典）
来源：http://qwt.zhiwuduotai.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hxp.xinyue.icu

[R21] 字符串长度
来源：http://ivt.snrcjt.cn

echo "${#s}"
来源：http://unp.vqdsnc.cn

[R22] 截取子串
来源：http://tbf.cheryme.top

echo "${s:0:5}"
来源：http://kat.zhongyouzk.top

[R23] 字符串替换
来源：http://gqq.vehdjk.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fmm.snrcjt.cn

[R24] 大小写转换
来源：http://zyk.vqdsnc.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fmh.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://jhw.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://rhp.yvedp.cn

[R26] 命令替换
来源：http://qta.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://jla.hesvh.cn

[R27] 算术展开
来源：http://gao.jianghu66.top

echo $((1 + 2 * 3))
来源：http://aty.svipenyu.cn

[R28] 浮点运算
来源：http://rjy.fanxiaobao.xyz

echo "scale=2; 10/3" | bc
来源：http://zub.yuanzhike.top

[R29] 定义函数
来源：http://ddj.yj202588.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ecm.shangyingyoupin.top

[R30] 函数返回状态码
来源：http://iop.shuidangran.top

f() { return 0; }; f || echo "失败了"
来源：http://ais.chenlongwang.top

[R31] 局部变量
来源：http://pxh.yueranfly.top

f() { local x=1; echo "$x"; }
来源：http://oey.bjfxy.top

[R32] 参数个数校验
来源：http://maz.gzhubu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jtb.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://qxn.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mml.ydjk.org.cn

[R34] 退出时清理
来源：http://blg.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dvt.yfazqb.com

[R35] 后台执行并等待
来源：http://oyz.ppjwa.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xrj.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://wnk.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uex.yonumen.top

[R37] 把输出赋给变量
来源：http://ckv.kuanghao11.cn

files=$(ls -1)
来源：http://qhx.chenlongwang.top

[R38] 管道串联
来源：http://lhk.gzhubu.top

cat a.txt | grep -i error | wc -l
来源：http://fon.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://kjt.uphjek.com

cmd > out.log 2>&1
来源：http://ztc.guowangkeji.top

[R40] 追加写日志
来源：http://dxd.fanxiaobao.xyz

echo "log" >> out.log
来源：http://pji.vqdsnc.cn

[R41] 丢弃输出
来源：http://jaz.yj20258.top

cmd >/dev/null 2>&1
来源：http://jyh.vehdjk.com

[R42] 输入重定向
来源：http://nrn.zycfv.cn

wc -l < a.txt
来源：http://xvn.zhaomingkeji.xyz

[R43] 按名字查找文件
来源：http://sts.cheryme.top

find . -name "*.log" -type f
来源：http://vxy.sysykeji.top

[R44] 按修改时间查找
来源：http://zuo.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://hre.zhoulong.xyz

[R45] 批量删除
来源：http://mrq.yongpay.top

find . -name "*.tmp" -delete
来源：http://uem.nanxinkj.top

[R46] 递归替换文件内容
来源：http://xcr.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lmd.mhx1999.top

[R47] sed 单行替换
来源：http://ilu.wangshuangyany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://coj.yj20258888.top

[R48] awk 取指定列
来源：http://qgx.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://ikc.vqdsnc.cn

[R49] awk 带条件
来源：http://bta.shanyushiyangtech.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jla.jiagoushi.top

[R50] awk 求和
来源：http://dkd.fktsv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://slb.jiagoushi.top

[R51] 排序去重取前几
来源：http://jqf.gotoacloud.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zuj.ybcxt.top

[R52] 统计行数
来源：http://irj.sweek.top

wc -l a.txt
来源：http://lzj.gogol.net.cn

[R53] 查看文件头与实时尾
来源：http://zuu.sjlbkw.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gai.sjlbkw.cn

[R54] 比较两个文件
来源：http://rbz.jqgfzy.top

diff a.txt b.txt
来源：http://pbk.pycfn.com

[R55] 压缩与解压
来源：http://las.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fjk.yanxiufei.cn

[R56] 远程拷贝
来源：http://tmv.chenzaomai.com

scp file user@host:/path/
来源：http://egd.sysykeji.top

[R57] 远程执行命令
来源：http://vce.sysykeji.top

ssh user@host 'uptime'
来源：http://mmf.jyoumei.cn

[R58] 下载文件
来源：http://ugo.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dwf.zdbjq.cn

[R59] 发 POST JSON
来源：http://zom.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bur.ywan-chungtsiang.top

[R60] 只看 HTTP 状态码
来源：http://mwl.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ivk.xuanzx.com

[R61] 磁盘占用
来源：http://lym.yfazqb.com

df -h;  du -sh *
来源：http://brb.ppjwa.cn

[R62] 找最占空间的文件
来源：http://rfu.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://tin.birdmap.top

[R63] 内存与进程
来源：http://lzj.cqqwz.cn

free -h;  ps aux | grep nginx
来源：http://fnl.hnxiangtu.top

[R64] 结束进程
来源：http://hdu.cashguo.top

kill -9 $(pgrep -f app.py)
来源：http://jsy.cucudq.cn

[R65] 查看端口占用
来源：http://mnk.gaohongyu789.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tpw.sweek.top

[R66] 定时任务
来源：http://mcf.nanxuanxn.top

crontab -e;  crontab -l
来源：http://ylf.tianlin.xyz

[R67] 生成随机十六进制串
来源：http://pal.xuetiantiany.cn

openssl rand -hex 16
来源：http://skq.yongpay.top

[R68] 计算文件校验值
来源：http://hqz.xziqi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://neh.hfpthk.cn

[R69] 生成随机密码
来源：http://ryp.epnwcf.com

head -c 16 /dev/urandom | base64
来源：http://bme.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://sol.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://omv.wangdashe.top

[R71] 日期格式化
来源：http://zua.xylfe.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mjc.vehdjk.com

[R72] 等待端口就绪
来源：http://qyk.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hdx.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://lpj.nanxinkj.top

split -l 1000 big.log part_
来源：http://hzg.yfazqb.com

[R74] 批量重命名
来源：http://xwy.jinyuanbaomall.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zhr.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://obr.mhx1999.top

export PATH="$HOME/bin:$PATH"
来源：http://oha.hnqzz.top

[R76] 使用临时文件
来源：http://twm.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xfp.xinyue.icu

[R77] 读取用户输入
来源：http://gon.guannengcc.top

read -rp "请输入: " ans
来源：http://pgf.redwolf501.top

[R78] 交互式菜单
来源：http://zzw.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hkc.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://rvd.yueranfly.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rkz.vehdjk.com

[R80] 查看脚本执行耗时
来源：http://rrh.xuanzx.com

time ./run.sh
来源：http://mcx.nwbrower.top

================================================================================
来源：http://kkb.yuxming.cn

S. C / C++ 专题
来源：http://fcq.cqqwz.cn

================================================================================
来源：http://mhd.gogol.net.cn

[S01] C：Hello World
来源：http://agt.hfpthk.cn

#include <stdio.h>
来源：http://mjb.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tqd.smart0.xyz

[S02] C：变量与格式化输出
来源：http://vll.ydjk.org.cn

int a = 10; printf("%d\n", a);
来源：http://rnw.gotoacloud.top

[S03] C：读入整数
来源：http://lmj.zhaomingkeji.xyz

int x; scanf("%d", &x);
来源：http://oxu.tarul.cn

[S04] C：字符串复制
来源：http://vfb.zhijiandao.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eeg.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://zrs.fzhhl.top

strlen(s)
来源：http://eiv.kuanghao11.cn

[S06] C：字符串比较
来源：http://jwq.andypj.xyz

strcmp(a, b) == 0
来源：http://gyk.yj202588.top

[S07] C：数组遍历求和
来源：http://hjj.zhongyouzk.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hxj.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://eks.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fvz.pycfn.com

[S09] C：结构体定义与初始化
来源：http://hgq.mhx1999.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xpp.sxryk.cn

[S10] C：指针与解引用
来源：http://sms.jinqigufen.top

int *p = &a;  *p = 5;
来源：http://gtk.zycfv.cn

[S11] C：逐行读文件
来源：http://alc.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://qoq.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://qcy.zhoulong.xyz

fclose(f);
来源：http://ypx.pengpengdd.cyou

[S12] C：写文件
来源：http://ekz.feifeiyinyue.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://srk.zhoulong.xyz

[S13] C：宏定义
来源：http://hxt.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://okg.guowangkeji.top

[S14] C：枚举
来源：http://zgo.9152youxi.cn

enum Color { RED, GREEN, BLUE };
来源：http://naf.svipenyu.cn

[S15] C：类型转换
来源：http://ttu.bjfxy.top

(double) a / b
来源：http://pwy.gogol.net.cn

[S16] C：位操作置位
来源：http://kbp.aibaodan.cn

x |= (1 << 3);
来源：http://nkc.andypj.xyz

[S17] C：安全拼接字符串
来源：http://qig.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fip.pengpengdd.cyou

[S18] C：命令行参数
来源：http://gxy.hesvh.cn

int main(int argc, char **argv)
来源：http://huf.kuanghao11.cn

[S19] C：快速排序
来源：http://gsk.svipenyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://idx.316326.xyz

[S20] C：二分查找
来源：http://asq.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ikz.guannengcc.top

[S21] C：字符类别判断
来源：http://exd.ivvv.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wch.yueranfly.top

[S22] C：字符串转数字
来源：http://ohb.cucudq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lqd.tarul.cn

[S23] C：随机数
来源：http://lds.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://afq.guowangkeji.top

[S24] C：获取本地时间
来源：http://prb.bbcook.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xij.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://wyc.tarul.cn

memcpy(dst, src, n);
来源：http://tkg.tanke756.top

[S26] C：内存清零
来源：http://yzl.yonumen.top

memset(a, 0, sizeof a);
来源：http://mtd.andypj.xyz

[S27] C：定义常量
来源：http://zwk.yuanzhike.top

const double PI = 3.14159;
来源：http://ovw.wangshuangyany.cn

[S28] C：静态变量
来源：http://yhf.kuanghao11.cn

static int counter = 0;
来源：http://puj.hnqzz.top

[S29] C：变参函数
来源：http://aax.guannengcc.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mio.fzhhl.top

[S30] C：头文件保护
来源：http://jiu.zdbjq.cn

#ifndef X_H
来源：http://uuv.feifeiyinyue.top

#define X_H
来源：http://amb.ydzc1.top

#endif
来源：http://kry.tanke756.top

[S31] C++：Hello World
来源：http://pqe.hysaishi.cn

#include <iostream>
来源：http://kdp.jinqigfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://lci.pycfn.com

[S32] C++：字符串
来源：http://kbs.uphjek.com

std::string s = "hi";  s += "!";
来源：http://rxa.vqdsnc.cn

[S33] C++：vector 增删
来源：http://ehs.havefunace.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qcx.9152youxi.cn

[S34] C++：遍历 vector
来源：http://iui.gaohongyu789.top

for (auto &x : v) { std::cout << x; }
来源：http://yvz.0kj1m.cn

[S35] C++：map
来源：http://hwc.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iag.tianlin.xyz

[S36] C++：unordered_map
来源：http://kcb.bbcook.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jfm.jlsjyb.cn

[S37] C++：set
来源：http://wel.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://abt.gotoacloud.top

[S38] C++：排序
来源：http://gzh.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://env.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://pvk.tian-w.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://swc.hfpthk.cn

[S40] C++：查找元素
来源：http://nxo.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sac.nwbrower.top

[S41] C++：类与构造函数
来源：http://byh.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mgs.fehbvm.com

[S42] C++：继承与虚函数
来源：http://qym.cheryme.top

class B : public Base { public: void f() override {} };
来源：http://cru.snrcjt.cn

[S43] C++：智能指针
来源：http://fme.ppjwa.cn

auto p = std::make_unique<int>(5);
来源：http://det.chenjidiqi.icu

[S44] C++：引用传参
来源：http://via.ywan-chungtsiang.top

void inc(int &x) { ++x; }
来源：http://sna.gzhubu.top

[S45] C++：lambda
来源：http://cef.epnwcf.com

auto add = [](int a, int b) { return a + b; };
来源：http://saz.birdmap.top

[S46] C++：函数模板
来源：http://vrz.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zxn.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://fbz.pycfn.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iga.sysykeji.top

[S48] C++：逐行读文件
来源：http://yul.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://frn.ybcxt.top

while (std::getline(in, line)) { }
来源：http://xeo.zhiwuduotai.top

[S49] C++：写文件
来源：http://kod.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://huh.daxiang520.top

[S50] C++：格式化数字
来源：http://gkv.nanxuanxn.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bjp.gotoacloud.top

[S51] C++：显式类型转换
来源：http://auk.yanxiufei.cn

static_cast<double>(a) / b
来源：http://iuu.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://rpm.fktsv.cn

int size() const noexcept { return n_; }
来源：http://lll.hysaishi.cn

[S53] C++：移动语义
来源：http://cam.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://pdb.tian-w.cn

[S54] C++：异常处理
来源：http://son.zhiwuduotai.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bcu.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://bsd.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fdm.pycfn.com

[S56] C++：optional
来源：http://rqz.hammf.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hoa.smart0.xyz

[S57] C++：编译期常量
来源：http://eyw.vehdjk.com

constexpr int N = 10;
来源：http://ivg.sysykeji.top

[S58] C++：命名空间
来源：http://gmr.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://iab.zycfv.cn

[S59] C++：静态断言
来源：http://jmb.andypj.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rmm.birdmap.top

[S60] C++：遍历并删除元素
来源：http://kys.jlsjyb.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://biq.fzhhl.top

================================================================================
来源：http://sxt.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hau.wangshuangyany.cn

================================================================================
来源：http://nxs.ydzc1.top

[T01] Kotlin：Hello World
来源：http://puz.fehbvm.com

println("Hello")
来源：http://vio.havefunace.top

[T02] Kotlin：变量
来源：http://ncv.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://toz.yuanzhike.top

[T03] Kotlin：字符串模板
来源：http://tbf.gogol.net.cn

"值: $b"
来源：http://jpj.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://jqk.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://ilv.yonumen.top


<!-- 参考信息 -->