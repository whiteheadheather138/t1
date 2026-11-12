代发 wailian999

readonly PI=3.14
来源：http://yvs.svipenyu.cn

[R04] 位置参数
来源：http://tjs.jlsjyb.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tax.shuidangran.top

[R05] 参数默认值
来源：http://fbb.jqgfzy.top

name="${1:-default}"
来源：http://ouv.xylfe.cn

[R06] 判断命令是否存在
来源：http://lbf.meibo888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://smu.feifeiyinyue.top

[R07] if 判断文件
来源：http://ezb.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dik.sjlbkw.cn

[R08] 数值比较
来源：http://mmh.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mod.yvedp.cn

[R09] 字符串比较
来源：http://pmo.yuanzhike.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://emd.cheryme.top

[R10] 正则匹配
来源：http://lxz.hammf.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://evs.chenlongwang.top

[R11] case 多分支
来源：http://bvu.sjlbkw.cn

case "$1" in
来源：http://tuq.fehbvm.com

start) echo "启动" ;;
来源：http://sgh.cucudq.cn

stop)  echo "停止" ;;
来源：http://mem.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://hid.chenlongwang.top

esac
来源：http://ohi.yj20258.top

[R12] for 遍历文件
来源：http://kir.bbcook.cn

for f in *.txt; do echo "$f"; done
来源：http://cjb.guannengcc.top

[R13] for 计数循环
来源：http://jfs.sweek.top

for i in {1..10}; do echo "$i"; done
来源：http://cql.quarkkingdee.top

[R14] C 风格 for
来源：http://nzq.ydjk.org.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cvp.nwbrower.top

[R15] while 逐行读文件
来源：http://oza.nanxuanxn.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bou.tianlin.xyz

[R16] until 等待条件
来源：http://vls.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://may.cdnleiting.top

[R17] 数组定义与取值
来源：http://ent.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://ehy.xinyue.icu

[R18] 遍历数组
来源：http://vfl.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cxy.yvedp.cn

[R19] 数组长度
来源：http://kcv.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://fcq.andypj.xyz

[R20] 关联数组（字典）
来源：http://zxq.zhoulong.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ovx.jinghuilouyu.cn

[R21] 字符串长度
来源：http://boj.yj20258888.top

echo "${#s}"
来源：http://oyc.ydjk.org.cn

[R22] 截取子串
来源：http://orv.hnxiangtu.top

echo "${s:0:5}"
来源：http://uqe.quarkkingdee.top

[R23] 字符串替换
来源：http://otp.tarul.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iss.yuanzhike.top

[R24] 大小写转换
来源：http://end.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://dac.svipenyu.cn

[R25] 去后缀 / 去前缀
来源：http://wjv.tian-w.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hph.gogol.net.cn

[R26] 命令替换
来源：http://sig.birdmap.top

now=$(date +%F); echo "$now"
来源：http://vuv.wangshuangyany.cn

[R27] 算术展开
来源：http://ndj.nwbrower.top

echo $((1 + 2 * 3))
来源：http://hqh.tianlin.xyz

[R28] 浮点运算
来源：http://wae.fehbvm.com

echo "scale=2; 10/3" | bc
来源：http://hqx.xziqi.cn

[R29] 定义函数
来源：http://ehl.yj202588.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kcw.jlsjyb.cn

[R30] 函数返回状态码
来源：http://myb.quarkkingdee.top

f() { return 0; }; f || echo "失败了"
来源：http://ifj.316326.xyz

[R31] 局部变量
来源：http://jsf.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://zdp.cashguo.top

[R32] 参数个数校验
来源：http://yqh.hammf.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fnu.ywan-chungtsiang.top

[R33] 捕获错误并提示行号
来源：http://dkv.jinqigfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://srk.dianchejie.cn

[R34] 退出时清理
来源：http://viq.9152youxi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rbk.0kj1m.cn

[R35] 后台执行并等待
来源：http://bcv.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://psh.zhongyouzk.top

[R36] 并发执行多个任务
来源：http://mvw.cdnleiting.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xdz.hesvh.cn

[R37] 把输出赋给变量
来源：http://ztd.chenlongwang.top

files=$(ls -1)
来源：http://poa.pycfn.com

[R38] 管道串联
来源：http://eye.vehdjk.com

cat a.txt | grep -i error | wc -l
来源：http://dxu.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://tyg.shanyushiyangkeji.top

cmd > out.log 2>&1
来源：http://mbj.cashguo.top

[R40] 追加写日志
来源：http://wdl.guannengcc.top

echo "log" >> out.log
来源：http://bcp.xuanzx.com

[R41] 丢弃输出
来源：http://gcb.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://tzh.jinyuanbaomall.cn

[R42] 输入重定向
来源：http://piq.shuidangran.top

wc -l < a.txt
来源：http://blv.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://nrl.yuxming.cn

find . -name "*.log" -type f
来源：http://jat.yvedp.cn

[R44] 按修改时间查找
来源：http://dkt.cqqwz.cn

find . -mtime -7 -type f
来源：http://rdm.ehwqpu.com

[R45] 批量删除
来源：http://yca.ivvv.top

find . -name "*.tmp" -delete
来源：http://ixw.daxiang520.top

[R46] 递归替换文件内容
来源：http://rlg.yuanzhike.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://niu.chenjidiqi.icu

[R47] sed 单行替换
来源：http://ljr.epnwcf.com

sed -i 's/foo/bar/g' a.txt
来源：http://lpn.ppjwa.cn

[R48] awk 取指定列
来源：http://ifz.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://yfi.zhoulong.xyz

[R49] awk 带条件
来源：http://xvr.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jyf.yangfankeji.com

[R50] awk 求和
来源：http://sfq.yj202588.top

awk '{s += $2} END {print s}' a.txt
来源：http://nph.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://ahs.haohaochexian.top

sort a.txt | uniq -c | sort -rn | head
来源：http://udo.xziqi.cn

[R52] 统计行数
来源：http://czu.c1oappe.top

wc -l a.txt
来源：http://cip.havefunace.top

[R53] 查看文件头与实时尾
来源：http://dmj.xuetiantiany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lmr.jlsjyb.cn

[R54] 比较两个文件
来源：http://dow.gzhubu.top

diff a.txt b.txt
来源：http://szr.52xcode.cn

[R55] 压缩与解压
来源：http://seh.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mwb.kuanghao11.cn

[R56] 远程拷贝
来源：http://yvo.nwbrower.top

scp file user@host:/path/
来源：http://saz.hnxiangtu.top

[R57] 远程执行命令
来源：http://apn.mhx1999.top

ssh user@host 'uptime'
来源：http://nio.sxryk.cn

[R58] 下载文件
来源：http://kvk.shangyingyoupin.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ssi.kuanghao11.cn

[R59] 发 POST JSON
来源：http://aos.redwolf501.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://alq.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://lev.316326.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yzc.bjfxy.top

[R61] 磁盘占用
来源：http://kyg.gzhubu.top

df -h;  du -sh *
来源：http://fqj.sweek.top

[R62] 找最占空间的文件
来源：http://hif.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://uzc.sjlbkw.cn

[R63] 内存与进程
来源：http://scl.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://idz.gzhubu.top

[R64] 结束进程
来源：http://tkm.andypj.xyz

kill -9 $(pgrep -f app.py)
来源：http://jtp.hnxiangtu.top

[R65] 查看端口占用
来源：http://dqu.nanxuanxn.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ytb.yongpay.top

[R66] 定时任务
来源：http://mda.yonumen.top

crontab -e;  crontab -l
来源：http://iot.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://hpo.yj20258.top

openssl rand -hex 16
来源：http://pyb.yangfankeji.com

[R68] 计算文件校验值
来源：http://ynw.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rsf.ivvv.top

[R69] 生成随机密码
来源：http://glc.snrcjt.cn

head -c 16 /dev/urandom | base64
来源：http://yyb.aibaodan.cn

[R70] 时间戳与互转
来源：http://txg.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://kdz.zdqjudy.top

[R71] 日期格式化
来源：http://rha.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lzd.nanxinkj.top

[R72] 等待端口就绪
来源：http://nbo.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fdl.xuanzx.com

[R73] 分割大日志
来源：http://jzd.guowangkeji.top

split -l 1000 big.log part_
来源：http://fzi.shangyingyoupin.top

[R74] 批量重命名
来源：http://apb.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://abk.yangfankeji.com

[R75] 导出环境变量
来源：http://gmu.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://czy.mhx1999.top

[R76] 使用临时文件
来源：http://llz.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://urk.gzhubu.top

[R77] 读取用户输入
来源：http://fsp.shanyushiyangkeji.top

read -rp "请输入: " ans
来源：http://jeu.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://ocq.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yjd.ppjwa.cn

[R79] 解析命令行选项
来源：http://hju.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://riz.vehdjk.com

[R80] 查看脚本执行耗时
来源：http://oti.pengpengdd.cyou

time ./run.sh
来源：http://lmb.zhaomingkeji.xyz

================================================================================
来源：http://xza.wangshuangyany.cn

S. C / C++ 专题
来源：http://vpj.fehbvm.com

================================================================================
来源：http://gqn.sufxvd.cn

[S01] C：Hello World
来源：http://udf.meibo888.top

#include <stdio.h>
来源：http://ysj.sufxvd.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tfu.redwolf501.top

[S02] C：变量与格式化输出
来源：http://qlx.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://gzz.iojbl.cn

[S03] C：读入整数
来源：http://goc.chenlongwang.top

int x; scanf("%d", &x);
来源：http://rkd.ybcxt.top

[S04] C：字符串复制
来源：http://jnw.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gfu.shzxlz.cn

[S05] C：字符串长度
来源：http://eca.nwbrower.top

strlen(s)
来源：http://iyg.xuetiantiany.cn

[S06] C：字符串比较
来源：http://yqe.gogol.net.cn

strcmp(a, b) == 0
来源：http://bbd.shuidangran.top

[S07] C：数组遍历求和
来源：http://mha.zhongyouzk.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ixe.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://smz.yj20258888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gnt.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://prv.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ewz.jiagoushi.top

[S10] C：指针与解引用
来源：http://cdy.tarul.cn

int *p = &a;  *p = 5;
来源：http://lia.vehdjk.com

[S11] C：逐行读文件
来源：http://bfw.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://ibc.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zil.daxiang520.top

fclose(f);
来源：http://ppu.bjfxy.top

[S12] C：写文件
来源：http://qza.zhengqikj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dyv.hfpthk.cn

[S13] C：宏定义
来源：http://ucw.yvedp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://llf.jinqigufen.top

[S14] C：枚举
来源：http://xjf.shzxlz.cn

enum Color { RED, GREEN, BLUE };
来源：http://hvw.ywan-chungtsiang.top

[S15] C：类型转换
来源：http://huz.hesvh.cn

(double) a / b
来源：http://wbb.zhaomingkeji.xyz

[S16] C：位操作置位
来源：http://suy.jinqigfzy.top

x |= (1 << 3);
来源：http://pyg.xziqi.cn

[S17] C：安全拼接字符串
来源：http://jkp.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ycf.zhijiandao.cn

[S18] C：命令行参数
来源：http://vgr.cqqwz.cn

int main(int argc, char **argv)
来源：http://wqo.pycfn.com

[S19] C：快速排序
来源：http://cvy.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xqd.zhixingplan.top

[S20] C：二分查找
来源：http://qtr.chenlongwang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mvy.jinghuilouyu.cn

[S21] C：字符类别判断
来源：http://vps.fehbvm.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lsb.quarkkingdee.top

[S22] C：字符串转数字
来源：http://afs.cucudq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rju.316326.xyz

[S23] C：随机数
来源：http://iyn.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bhx.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://nvc.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ugs.epnwcf.com

[S25] C：内存拷贝
来源：http://zmd.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://jng.tian-w.cn

[S26] C：内存清零
来源：http://ynf.hesvh.cn

memset(a, 0, sizeof a);
来源：http://svz.52xcode.cn

[S27] C：定义常量
来源：http://fnb.shangyingyoupin.top

const double PI = 3.14159;
来源：http://vhm.yangfankeji.com

[S28] C：静态变量
来源：http://hpy.sxryk.cn

static int counter = 0;
来源：http://fgy.epnwcf.com

[S29] C：变参函数
来源：http://cjg.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bpo.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://mtk.jqgufenzy.top

#ifndef X_H
来源：http://gva.zdqjudy.top

#define X_H
来源：http://quk.cqqwz.cn

#endif
来源：http://hco.ywan-chungtsiang.top

[S31] C++：Hello World
来源：http://wpa.daria6918.cn

#include <iostream>
来源：http://ewm.jinqigufen.top

int main() { std::cout << "Hello\n"; }
来源：http://sft.yj202588.top

[S32] C++：字符串
来源：http://lfs.jinqigfzy.top

std::string s = "hi";  s += "!";
来源：http://ocl.snrcjt.cn

[S33] C++：vector 增删
来源：http://ihm.fktsv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ngs.yvedp.cn

[S34] C++：遍历 vector
来源：http://hov.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://gzd.iojbl.cn

[S35] C++：map
来源：http://tuu.zhoulong.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xhn.cheryme.top

[S36] C++：unordered_map
来源：http://nxa.ppjwa.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://odg.sweek.top

[S37] C++：set
来源：http://yle.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lpx.hcnkem.com

[S38] C++：排序
来源：http://cbq.birdmap.top

std::sort(v.begin(), v.end());
来源：http://psp.vqdsnc.cn

[S39] C++：自定义比较器排序
来源：http://xzt.gotoacloud.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kxv.sxryk.cn

[S40] C++：查找元素
来源：http://yae.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nso.zdbjq.cn

[S41] C++：类与构造函数
来源：http://cui.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kjt.hammf.cn

[S42] C++：继承与虚函数
来源：http://vnz.cashguo.top

class B : public Base { public: void f() override {} };
来源：http://kug.cqqwz.cn

[S43] C++：智能指针
来源：http://bxw.cqqwz.cn

auto p = std::make_unique<int>(5);
来源：http://suc.gaohongyu789.top

[S44] C++：引用传参
来源：http://dqu.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://zal.wangdashe.top

[S45] C++：lambda
来源：http://lxf.ehwqpu.com

auto add = [](int a, int b) { return a + b; };
来源：http://jtm.xuetiantiany.cn

[S46] C++：函数模板
来源：http://jbx.nanxinkj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yyt.zdqjudy.top

[S47] C++：结构化绑定遍历
来源：http://mbd.316326.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kpv.jyoumei.cn

[S48] C++：逐行读文件
来源：http://tip.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://qix.yuxming.cn

while (std::getline(in, line)) { }
来源：http://rmr.gzhubu.top

[S49] C++：写文件
来源：http://umt.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xga.yvedp.cn

[S50] C++：格式化数字
来源：http://xwi.sweek.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://swq.52xcode.cn

[S51] C++：显式类型转换
来源：http://rbz.cucudq.cn

static_cast<double>(a) / b
来源：http://yzd.jyoumei.cn

[S52] C++：const 与 noexcept
来源：http://eqe.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://bsb.bbcook.cn

[S53] C++：移动语义
来源：http://peu.iojbl.cn

std::vector<int> w = std::move(v);
来源：http://zmt.jyoumei.cn

[S54] C++：异常处理
来源：http://lcf.yueranfly.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lia.daxiang520.top

[S55] C++：结构化绑定
来源：http://zzn.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://okv.yfazqb.com

[S56] C++：optional
来源：http://mcd.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vkx.daria6918.cn

[S57] C++：编译期常量
来源：http://iod.0kj1m.cn

constexpr int N = 10;
来源：http://nsu.hongshengwenyu.top

[S58] C++：命名空间
来源：http://mhr.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://ght.fehbvm.com

[S59] C++：静态断言
来源：http://icu.kuanghao11.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pyk.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://bwl.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cze.zdbjq.cn

================================================================================
来源：http://nol.c1oappe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ryq.chenlongwang.top

================================================================================
来源：http://icr.redwolf501.top

[T01] Kotlin：Hello World
来源：http://hhm.shuidangran.top

println("Hello")
来源：http://lft.jinqigufen.top

[T02] Kotlin：变量
来源：http://yqg.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sxa.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://aku.chenlongwang.top

"值: $b"
来源：http://tfb.quarkkingdee.top

[T04] Kotlin：空安全
来源：http://bzn.ivvv.top

val n: String? = null;  n?.length
来源：http://xxl.0kj1m.cn


<!-- 参考信息 -->