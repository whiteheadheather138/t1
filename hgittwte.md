代发 wailian999

set -euo pipefail
来源：http://sht.ppjwa.cn

[R02] 变量赋值与使用
来源：http://gsg.kuanghao11.cn

name="Tom"; echo "$name"
来源：http://zqv.zhixingplan.top

[R03] 只读变量
来源：http://fdn.wangshuangyany.cn

readonly PI=3.14
来源：http://qew.hammf.cn

[R04] 位置参数
来源：http://ocl.cdnleiting.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zoo.nanxuanxn.top

[R05] 参数默认值
来源：http://qrw.cdnleiting.top

name="${1:-default}"
来源：http://aaa.bjfxy.top

[R06] 判断命令是否存在
来源：http://dce.vehdjk.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ezf.sysykeji.top

[R07] if 判断文件
来源：http://zhu.dianchejie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qjs.jiagoushi.top

[R08] 数值比较
来源：http://etr.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jdz.bjfxy.top

[R09] 字符串比较
来源：http://nej.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fsf.havefunace.top

[R10] 正则匹配
来源：http://lsy.jlsjyb.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mej.nanxuanxn.top

[R11] case 多分支
来源：http://txt.zhongyouzk.top

case "$1" in
来源：http://qth.yongpay.top

start) echo "启动" ;;
来源：http://jau.dianchejie.cn

stop)  echo "停止" ;;
来源：http://lwq.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://uwr.0kj1m.cn

esac
来源：http://tlg.cashguo.top

[R12] for 遍历文件
来源：http://bra.nanxinkj.top

for f in *.txt; do echo "$f"; done
来源：http://zfu.vqdsnc.cn

[R13] for 计数循环
来源：http://rqb.quarkkingdee.top

for i in {1..10}; do echo "$i"; done
来源：http://zmt.shanyushiyangkeji.top

[R14] C 风格 for
来源：http://wlk.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://suf.guowangkeji.top

[R15] while 逐行读文件
来源：http://ere.sweek.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oge.yanxiufei.cn

[R16] until 等待条件
来源：http://zpn.birdmap.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rfd.wangdashe.top

[R17] 数组定义与取值
来源：http://wxg.yonumen.top

arr=(a b c); echo "${arr[0]}"
来源：http://bxu.jinyuanbaomall.cn

[R18] 遍历数组
来源：http://czj.zhaomingkeji.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hsp.daria6918.cn

[R19] 数组长度
来源：http://uri.gotoacloud.top

echo "${#arr[@]}"
来源：http://zym.hnqzz.top

[R20] 关联数组（字典）
来源：http://sjc.hnqzz.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gqa.zhengqikj.top

[R21] 字符串长度
来源：http://zdk.yfazqb.com

echo "${#s}"
来源：http://gwx.pycfn.com

[R22] 截取子串
来源：http://abd.dianchejie.cn

echo "${s:0:5}"
来源：http://iaz.ydzc1.top

[R23] 字符串替换
来源：http://ghu.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sjc.bbcook.cn

[R24] 大小写转换
来源：http://vev.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ude.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://izx.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cat.cheryme.top

[R26] 命令替换
来源：http://nlb.pengpengdd.cyou

now=$(date +%F); echo "$now"
来源：http://mca.sxryk.cn

[R27] 算术展开
来源：http://aia.daria6918.cn

echo $((1 + 2 * 3))
来源：http://zgh.jyoumei.cn

[R28] 浮点运算
来源：http://dnz.pengpengdd.cyou

echo "scale=2; 10/3" | bc
来源：http://rot.yvedp.cn

[R29] 定义函数
来源：http://brm.hfpthk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pbv.zhijiandao.cn

[R30] 函数返回状态码
来源：http://rxt.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://yqf.ivvv.top

[R31] 局部变量
来源：http://mgu.andypj.xyz

f() { local x=1; echo "$x"; }
来源：http://hhw.guowangkeji.top

[R32] 参数个数校验
来源：http://hdr.andypj.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pwz.yanxiufei.cn

[R33] 捕获错误并提示行号
来源：http://sga.yfazqb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://veq.tanke756.top

[R34] 退出时清理
来源：http://ttk.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://hld.fehbvm.com

[R35] 后台执行并等待
来源：http://aup.svipenyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://btu.bjfxy.top

[R36] 并发执行多个任务
来源：http://ykw.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://icl.shzxlz.cn

[R37] 把输出赋给变量
来源：http://vou.ybcxt.top

files=$(ls -1)
来源：http://ose.jinqigufen.top

[R38] 管道串联
来源：http://kxp.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://qdw.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://cps.ehwqpu.com

cmd > out.log 2>&1
来源：http://lks.ppjwa.cn

[R40] 追加写日志
来源：http://gxd.haohaochexian.top

echo "log" >> out.log
来源：http://frd.birdmap.top

[R41] 丢弃输出
来源：http://rwd.ydzc1.top

cmd >/dev/null 2>&1
来源：http://odq.hnqzz.top

[R42] 输入重定向
来源：http://rxh.hammf.cn

wc -l < a.txt
来源：http://bpi.hesvh.cn

[R43] 按名字查找文件
来源：http://rhn.vehdjk.com

find . -name "*.log" -type f
来源：http://ovy.hnxiangtu.top

[R44] 按修改时间查找
来源：http://rwu.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://jzx.chenlongwang.top

[R45] 批量删除
来源：http://giy.jiagoushi.top

find . -name "*.tmp" -delete
来源：http://cka.fktsv.cn

[R46] 递归替换文件内容
来源：http://oyt.xuanzx.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xcq.meibo888.top

[R47] sed 单行替换
来源：http://lmt.xziqi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jfz.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://mnm.yonumen.top

awk '{print $1, $3}' a.txt
来源：http://tjk.fzhhl.top

[R49] awk 带条件
来源：http://pqy.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cxd.ydzc1.top

[R50] awk 求和
来源：http://uwx.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://xls.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://dkl.aibaodan.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hnv.zhaomingkeji.xyz

[R52] 统计行数
来源：http://bcd.haohaochexian.top

wc -l a.txt
来源：http://ddi.zhiwuduotai.top

[R53] 查看文件头与实时尾
来源：http://jln.sysykeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://toe.gaohongyu789.top

[R54] 比较两个文件
来源：http://whc.chenjidiqi.icu

diff a.txt b.txt
来源：http://yxr.fehbvm.com

[R55] 压缩与解压
来源：http://wkb.vqdsnc.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ivj.316326.xyz

[R56] 远程拷贝
来源：http://jql.ppjwa.cn

scp file user@host:/path/
来源：http://lhh.sxryk.cn

[R57] 远程执行命令
来源：http://nky.havefunace.top

ssh user@host 'uptime'
来源：http://emy.nwbrower.top

[R58] 下载文件
来源：http://mng.fktsv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sxr.yonumen.top

[R59] 发 POST JSON
来源：http://bqr.ctjpmb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vpm.jlsjyb.cn

[R60] 只看 HTTP 状态码
来源：http://gcy.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gra.mhx1999.top

[R61] 磁盘占用
来源：http://ffu.haohaochexian.top

df -h;  du -sh *
来源：http://azp.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://xsr.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://lkx.fehbvm.com

[R63] 内存与进程
来源：http://coc.bjfxy.top

free -h;  ps aux | grep nginx
来源：http://rlv.0kj1m.cn

[R64] 结束进程
来源：http://jsb.pycfn.com

kill -9 $(pgrep -f app.py)
来源：http://rmt.316326.xyz

[R65] 查看端口占用
来源：http://uas.zhaomingkeji.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xcl.jqgfzy.top

[R66] 定时任务
来源：http://kvk.havefunace.top

crontab -e;  crontab -l
来源：http://nhx.tianlin.xyz

[R67] 生成随机十六进制串
来源：http://aiu.hcnkem.com

openssl rand -hex 16
来源：http://lsn.smart0.xyz

[R68] 计算文件校验值
来源：http://ndb.ydzc1.top

sha256sum a.txt;  md5sum a.txt
来源：http://btz.jqgufenzy.top

[R69] 生成随机密码
来源：http://zre.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://rkv.ydzc1.top

[R70] 时间戳与互转
来源：http://nwx.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://asf.yj20258.top

[R71] 日期格式化
来源：http://byp.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zjn.vehdjk.com

[R72] 等待端口就绪
来源：http://gye.hywenlv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pjn.jianghu66.top

[R73] 分割大日志
来源：http://zfq.shzxlz.cn

split -l 1000 big.log part_
来源：http://qxm.hnqzz.top

[R74] 批量重命名
来源：http://xfi.guannengcc.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lad.feifeiyinyue.top

[R75] 导出环境变量
来源：http://vxv.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://hud.yongpay.top

[R76] 使用临时文件
来源：http://hkn.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mxi.ctjpmb.com

[R77] 读取用户输入
来源：http://rsz.zhixingplan.top

read -rp "请输入: " ans
来源：http://kxt.kuanghao11.cn

[R78] 交互式菜单
来源：http://ums.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://ghw.xziqi.cn

[R79] 解析命令行选项
来源：http://tub.hysaishi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yqb.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://vwq.zhaomingkeji.xyz

time ./run.sh
来源：http://knj.zhijiandao.cn

================================================================================
来源：http://vdt.uphjek.com

S. C / C++ 专题
来源：http://lnz.yuxming.cn

================================================================================
来源：http://vyp.jqgufenzy.top

[S01] C：Hello World
来源：http://ibg.sjlbkw.cn

#include <stdio.h>
来源：http://rrr.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://eee.fehbvm.com

[S02] C：变量与格式化输出
来源：http://gjc.nanxuanxn.top

int a = 10; printf("%d\n", a);
来源：http://nmh.zdbjq.cn

[S03] C：读入整数
来源：http://jfj.tanke756.top

int x; scanf("%d", &x);
来源：http://dyf.hywenlv.cn

[S04] C：字符串复制
来源：http://cbv.fanxiaobao.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://sbx.hfpthk.cn

[S05] C：字符串长度
来源：http://iyi.shangyingyoupin.top

strlen(s)
来源：http://mqt.zhoulong.xyz

[S06] C：字符串比较
来源：http://uxb.guowangkeji.top

strcmp(a, b) == 0
来源：http://zbc.vehdjk.com

[S07] C：数组遍历求和
来源：http://xxk.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wdx.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://isg.shanyushiyangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wvp.316326.xyz

[S09] C：结构体定义与初始化
来源：http://ojp.sufxvd.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sph.hammf.cn

[S10] C：指针与解引用
来源：http://txd.tarul.cn

int *p = &a;  *p = 5;
来源：http://cil.zhongyouzk.top

[S11] C：逐行读文件
来源：http://gks.aizwys.cn

FILE *f = fopen("a.txt", "r");
来源：http://exu.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://moi.sjlbkw.cn

fclose(f);
来源：http://zys.andypj.xyz

[S12] C：写文件
来源：http://ovo.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ujx.ivvv.top

[S13] C：宏定义
来源：http://jyg.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lho.epnwcf.com

[S14] C：枚举
来源：http://zwf.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://uvf.dianchejie.cn

[S15] C：类型转换
来源：http://wnh.52xcode.cn

(double) a / b
来源：http://hzx.hywenlv.cn

[S16] C：位操作置位
来源：http://hwt.cucudq.cn

x |= (1 << 3);
来源：http://drn.tarul.cn

[S17] C：安全拼接字符串
来源：http://qjm.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qcp.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://cry.fengsongda.top

int main(int argc, char **argv)
来源：http://xqx.guowangkeji.top

[S19] C：快速排序
来源：http://lug.jinyuanbaomall.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ckq.feifeiyinyue.top

[S20] C：二分查找
来源：http://tez.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pzb.havefunace.top

[S21] C：字符类别判断
来源：http://gjd.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mrd.tianlin.xyz

[S22] C：字符串转数字
来源：http://cgi.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rse.xylfe.cn

[S23] C：随机数
来源：http://pzb.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mfx.hesvh.cn

[S24] C：获取本地时间
来源：http://zpw.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dhc.jianghu66.top

[S25] C：内存拷贝
来源：http://czu.yangfankeji.com

memcpy(dst, src, n);
来源：http://tbe.epnwcf.com

[S26] C：内存清零
来源：http://ghl.fehbvm.com

memset(a, 0, sizeof a);
来源：http://zud.nanxinkj.top

[S27] C：定义常量
来源：http://dqa.fzhhl.top

const double PI = 3.14159;
来源：http://kaf.hnqzz.top

[S28] C：静态变量
来源：http://adg.yueranfly.top

static int counter = 0;
来源：http://tgb.gogol.net.cn

[S29] C：变参函数
来源：http://ewu.316326.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sbh.yj20258.top

[S30] C：头文件保护
来源：http://ltz.0kj1m.cn

#ifndef X_H
来源：http://pek.jinghuilouyu.cn

#define X_H
来源：http://ckh.snrcjt.cn

#endif
来源：http://czo.havefunace.top

[S31] C++：Hello World
来源：http://crl.yueranfly.top

#include <iostream>
来源：http://pjw.ydjk.org.cn

int main() { std::cout << "Hello\n"; }
来源：http://wiv.redwolf501.top

[S32] C++：字符串
来源：http://qvr.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://xmu.smart0.xyz

[S33] C++：vector 增删
来源：http://rce.yongpay.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vwj.feifeiyinyue.top

[S34] C++：遍历 vector
来源：http://lhf.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://rjj.gogol.net.cn

[S35] C++：map
来源：http://pwx.ehwqpu.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ven.sweek.top

[S36] C++：unordered_map
来源：http://gbh.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kpf.hfpthk.cn

[S37] C++：set
来源：http://fht.yj20258.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cqc.shangyingyoupin.top

[S38] C++：排序
来源：http://kjq.ppjwa.cn

std::sort(v.begin(), v.end());
来源：http://ekm.hammf.cn

[S39] C++：自定义比较器排序
来源：http://thj.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pza.kuanghao11.cn

[S40] C++：查找元素
来源：http://qzo.ydzc1.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fil.sufxvd.cn

[S41] C++：类与构造函数
来源：http://wfy.zhengqikj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pkt.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://svg.jinqigfzy.top

class B : public Base { public: void f() override {} };
来源：http://npt.sweek.top

[S43] C++：智能指针
来源：http://khf.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://wju.meibo888.top

[S44] C++：引用传参
来源：http://xvp.yuanzhike.top

void inc(int &x) { ++x; }
来源：http://wud.yj202588.top

[S45] C++：lambda
来源：http://olt.ywan-chungtsiang.top

auto add = [](int a, int b) { return a + b; };
来源：http://vme.yj20258.top

[S46] C++：函数模板
来源：http://jto.jinyuanbaomall.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://igf.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://ddl.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vjl.zdqjudy.top

[S48] C++：逐行读文件
来源：http://tww.aizwys.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yal.xingfuxueyuan.xyz

while (std::getline(in, line)) { }
来源：http://mlk.haohaochexian.top

[S49] C++：写文件
来源：http://bpr.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sqn.svipenyu.cn

[S50] C++：格式化数字
来源：http://kcd.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dbs.hysaishi.cn

[S51] C++：显式类型转换
来源：http://sze.tian-w.cn

static_cast<double>(a) / b
来源：http://zco.hesvh.cn

[S52] C++：const 与 noexcept
来源：http://fkj.hongshengwenyu.top

int size() const noexcept { return n_; }
来源：http://lbr.ydzc1.top

[S53] C++：移动语义
来源：http://alo.chenzaomai.com

std::vector<int> w = std::move(v);
来源：http://ssm.hesvh.cn

[S54] C++：异常处理
来源：http://xhq.tanke756.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://luy.hywenlv.cn

[S55] C++：结构化绑定
来源：http://gmo.ydzc1.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dho.cucudq.cn

[S56] C++：optional
来源：http://zqt.yuanzhike.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yyh.zhaomingkeji.xyz

[S57] C++：编译期常量
来源：http://nek.jqgufenzy.top

constexpr int N = 10;
来源：http://byk.zycfv.cn

[S58] C++：命名空间
来源：http://kbg.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://dwv.zdbjq.cn

[S59] C++：静态断言
来源：http://wfk.guowangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yuj.tanke756.top

[S60] C++：遍历并删除元素
来源：http://fvc.xziqi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gfl.ehwqpu.com

================================================================================
来源：http://gcl.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zaf.gotoacloud.top

================================================================================
来源：http://blc.cdnleiting.top

[T01] Kotlin：Hello World
来源：http://qpi.ybcxt.top

println("Hello")
来源：http://ufv.sxryk.cn

[T02] Kotlin：变量
来源：http://peu.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bux.jiagoushi.top


<!-- 参考信息 -->