代发 wailian999

R. Bash 专题
来源：http://rbq.gaohongyu789.top

================================================================================
来源：http://xib.aizwys.cn

[R01] shebang 与严格模式
来源：http://lux.chenlongwang.top

#!/usr/bin/env bash
来源：http://dvs.zhengqikj.top

set -euo pipefail
来源：http://mqo.gogol.net.cn

[R02] 变量赋值与使用
来源：http://gdx.ehwqpu.com

name="Tom"; echo "$name"
来源：http://uoq.yj20258888.top

[R03] 只读变量
来源：http://rvs.quarkkingdee.top

readonly PI=3.14
来源：http://tqj.kuanghao11.cn

[R04] 位置参数
来源：http://xbg.haohaochexian.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yfc.yj202588.top

[R05] 参数默认值
来源：http://uls.fehbvm.com

name="${1:-default}"
来源：http://buy.ybcxt.top

[R06] 判断命令是否存在
来源：http://rqy.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cey.9152youxi.cn

[R07] if 判断文件
来源：http://ehd.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fjn.cqqwz.cn

[R08] 数值比较
来源：http://krb.birdmap.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jqi.nanxinkj.top

[R09] 字符串比较
来源：http://gnl.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gek.iojbl.cn

[R10] 正则匹配
来源：http://pyy.mhx1999.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cfx.gotoacloud.top

[R11] case 多分支
来源：http://qqs.jinqigfzy.top

case "$1" in
来源：http://jwt.hcnkem.com

start) echo "启动" ;;
来源：http://wxz.yvedp.cn

stop)  echo "停止" ;;
来源：http://sso.gogol.net.cn

*)     echo "未知命令" ;;
来源：http://lvx.jyoumei.cn

esac
来源：http://xin.pycfn.com

[R12] for 遍历文件
来源：http://zvs.fehbvm.com

for f in *.txt; do echo "$f"; done
来源：http://ayr.vqdsnc.cn

[R13] for 计数循环
来源：http://uwp.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://iik.daxiang520.top

[R14] C 风格 for
来源：http://qsj.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aay.guowangkeji.top

[R15] while 逐行读文件
来源：http://jhz.dashuyun.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vva.vehdjk.com

[R16] until 等待条件
来源：http://ecc.jianghu66.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gci.jlsjyb.cn

[R17] 数组定义与取值
来源：http://hyx.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kbd.hongshengwenyu.top

[R18] 遍历数组
来源：http://yqh.yj202588.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://krx.cqqwz.cn

[R19] 数组长度
来源：http://jhc.redwolf501.top

echo "${#arr[@]}"
来源：http://hjt.iojbl.cn

[R20] 关联数组（字典）
来源：http://fvb.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wjy.ctjpmb.com

[R21] 字符串长度
来源：http://mbh.xuanzx.com

echo "${#s}"
来源：http://eyb.tian-w.cn

[R22] 截取子串
来源：http://wpz.ivvv.top

echo "${s:0:5}"
来源：http://pdu.yj202588.top

[R23] 字符串替换
来源：http://rie.chenlongwang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fds.c1oappe.top

[R24] 大小写转换
来源：http://yjo.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://yxw.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://tyh.jqgufenzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://saq.jlsjyb.cn

[R26] 命令替换
来源：http://pwy.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://mgb.jqgufenzy.top

[R27] 算术展开
来源：http://sfo.ydzc1.top

echo $((1 + 2 * 3))
来源：http://qsl.zhijiandao.cn

[R28] 浮点运算
来源：http://mla.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://dbq.zhiwuduotai.top

[R29] 定义函数
来源：http://jaj.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ttg.nwbrower.top

[R30] 函数返回状态码
来源：http://ycu.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://mnv.jyoumei.cn

[R31] 局部变量
来源：http://uap.guannengcc.top

f() { local x=1; echo "$x"; }
来源：http://scx.52xcode.cn

[R32] 参数个数校验
来源：http://yiy.zhoulong.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uvm.chenjidiqi.icu

[R33] 捕获错误并提示行号
来源：http://dxd.svipenyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ypy.cdnleiting.top

[R34] 退出时清理
来源：http://loz.yueranfly.top

trap 'rm -f "$tmp"' EXIT
来源：http://hov.yj20258.top

[R35] 后台执行并等待
来源：http://lli.shzxlz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hht.pengpengdd.cyou

[R36] 并发执行多个任务
来源：http://pcg.vqdsnc.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oot.haohaochexian.top

[R37] 把输出赋给变量
来源：http://eot.ybcxt.top

files=$(ls -1)
来源：http://ger.ivvv.top

[R38] 管道串联
来源：http://sau.shuidangran.top

cat a.txt | grep -i error | wc -l
来源：http://rfo.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://hav.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://biz.ybcxt.top

[R40] 追加写日志
来源：http://fan.birdmap.top

echo "log" >> out.log
来源：http://jae.jqgfzy.top

[R41] 丢弃输出
来源：http://woe.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://vxj.tianlin.xyz

[R42] 输入重定向
来源：http://ygk.jlsjyb.cn

wc -l < a.txt
来源：http://fhz.fktsv.cn

[R43] 按名字查找文件
来源：http://idn.ywan-chungtsiang.top

find . -name "*.log" -type f
来源：http://sin.tianlin.xyz

[R44] 按修改时间查找
来源：http://grm.birdmap.top

find . -mtime -7 -type f
来源：http://aib.chenlongwang.top

[R45] 批量删除
来源：http://nwl.vehdjk.com

find . -name "*.tmp" -delete
来源：http://fjj.sweek.top

[R46] 递归替换文件内容
来源：http://lwt.pycfn.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://goq.jqgufenzy.top

[R47] sed 单行替换
来源：http://mtp.smart0.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://bwm.wangdashe.top

[R48] awk 取指定列
来源：http://pev.tanke756.top

awk '{print $1, $3}' a.txt
来源：http://ywf.snrcjt.cn

[R49] awk 带条件
来源：http://ngt.52xcode.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aql.ybcxt.top

[R50] awk 求和
来源：http://suw.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://efe.uphjek.com

[R51] 排序去重取前几
来源：http://jvd.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cvj.mhx1999.top

[R52] 统计行数
来源：http://zvb.bjfxy.top

wc -l a.txt
来源：http://yxg.chenzaomai.com

[R53] 查看文件头与实时尾
来源：http://rpv.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://irw.yanxiufei.cn

[R54] 比较两个文件
来源：http://kqi.wangshuangyany.cn

diff a.txt b.txt
来源：http://ofw.shuidangran.top

[R55] 压缩与解压
来源：http://mzq.hnqzz.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cmy.havefunace.top

[R56] 远程拷贝
来源：http://euu.daria6918.cn

scp file user@host:/path/
来源：http://mti.jyoumei.cn

[R57] 远程执行命令
来源：http://mtv.yj202588.top

ssh user@host 'uptime'
来源：http://ocy.kuanghao11.cn

[R58] 下载文件
来源：http://tgp.zhongyouzk.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bhl.xingfuxueyuan.xyz

[R59] 发 POST JSON
来源：http://tie.jinghuilouyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wge.cdnleiting.top

[R60] 只看 HTTP 状态码
来源：http://xeg.hcnkem.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://huo.andypj.xyz

[R61] 磁盘占用
来源：http://xrm.xylfe.cn

df -h;  du -sh *
来源：http://ibf.yfazqb.com

[R62] 找最占空间的文件
来源：http://jfj.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://hrk.shanyushiyangtech.top

[R63] 内存与进程
来源：http://pjq.nanxuanxn.top

free -h;  ps aux | grep nginx
来源：http://ery.daria6918.cn

[R64] 结束进程
来源：http://cuu.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://xyz.sufxvd.cn

[R65] 查看端口占用
来源：http://zoo.hnqzz.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yaa.yj202588.top

[R66] 定时任务
来源：http://dyy.bbcook.cn

crontab -e;  crontab -l
来源：http://lhf.hnqzz.top

[R67] 生成随机十六进制串
来源：http://ube.yanxiufei.cn

openssl rand -hex 16
来源：http://cor.gaohongyu789.top

[R68] 计算文件校验值
来源：http://zmn.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ovw.tarul.cn

[R69] 生成随机密码
来源：http://wvj.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://dsv.jinghuilouyu.cn

[R70] 时间戳与互转
来源：http://wnk.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://uyl.hnxiangtu.top

[R71] 日期格式化
来源：http://iqz.ehwqpu.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://rrp.cdnleiting.top

[R72] 等待端口就绪
来源：http://wpo.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ucl.yueranfly.top

[R73] 分割大日志
来源：http://ynu.yj202588.top

split -l 1000 big.log part_
来源：http://uut.hywenlv.cn

[R74] 批量重命名
来源：http://dhl.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lwk.ppjwa.cn

[R75] 导出环境变量
来源：http://tos.hammf.cn

export PATH="$HOME/bin:$PATH"
来源：http://pee.mhx1999.top

[R76] 使用临时文件
来源：http://zio.sufxvd.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kln.fzhhl.top

[R77] 读取用户输入
来源：http://gnz.xinyue.icu

read -rp "请输入: " ans
来源：http://neq.shangyingyoupin.top

[R78] 交互式菜单
来源：http://gvr.nanxinkj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mun.bjfxy.top

[R79] 解析命令行选项
来源：http://eqf.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://duz.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://svc.bjfxy.top

time ./run.sh
来源：http://ahv.smart0.xyz

================================================================================
来源：http://ebt.fehbvm.com

S. C / C++ 专题
来源：http://pxz.tianlin.xyz

================================================================================
来源：http://lan.hysaishi.cn

[S01] C：Hello World
来源：http://bpo.zdbjq.cn

#include <stdio.h>
来源：http://fle.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mtw.meibo888.top

[S02] C：变量与格式化输出
来源：http://goe.nanxuanxn.top

int a = 10; printf("%d\n", a);
来源：http://doy.cdnleiting.top

[S03] C：读入整数
来源：http://gkx.gogol.net.cn

int x; scanf("%d", &x);
来源：http://gyj.zhijiandao.cn

[S04] C：字符串复制
来源：http://ksr.aibaodan.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eir.cqqwz.cn

[S05] C：字符串长度
来源：http://rjg.ehwqpu.com

strlen(s)
来源：http://lhw.xuetiantiany.cn

[S06] C：字符串比较
来源：http://bpr.svipenyu.cn

strcmp(a, b) == 0
来源：http://dmm.yvedp.cn

[S07] C：数组遍历求和
来源：http://fwe.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://skt.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://tpw.ydjk.org.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xla.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://kys.aizwys.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://suy.zycfv.cn

[S10] C：指针与解引用
来源：http://wbe.hfpthk.cn

int *p = &a;  *p = 5;
来源：http://ujd.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://csr.svipenyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://rvj.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zvc.hnqzz.top

fclose(f);
来源：http://qan.tian-w.cn

[S12] C：写文件
来源：http://zwe.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zpv.vqdsnc.cn

[S13] C：宏定义
来源：http://pbz.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hmq.52xcode.cn

[S14] C：枚举
来源：http://nuq.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://lvy.sjlbkw.cn

[S15] C：类型转换
来源：http://jnn.jlsjyb.cn

(double) a / b
来源：http://tuq.fengsongda.top

[S16] C：位操作置位
来源：http://btx.feifeiyinyue.top

x |= (1 << 3);
来源：http://ovf.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://dni.shanyushiyangtech.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nhp.hesvh.cn

[S18] C：命令行参数
来源：http://itk.hnxiangtu.top

int main(int argc, char **argv)
来源：http://kta.yj202588.top

[S19] C：快速排序
来源：http://nul.jinqigufen.top

qsort(a, n, sizeof(int), cmp);
来源：http://lev.sxryk.cn

[S20] C：二分查找
来源：http://cej.guowangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gle.nwbrower.top

[S21] C：字符类别判断
来源：http://nbe.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vpr.hfpthk.cn

[S22] C：字符串转数字
来源：http://tiv.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://doq.yfazqb.com

[S23] C：随机数
来源：http://cjo.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xug.guowangkeji.top

[S24] C：获取本地时间
来源：http://iar.zycfv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xfm.hesvh.cn

[S25] C：内存拷贝
来源：http://gac.yj20258888.top

memcpy(dst, src, n);
来源：http://ouw.sxryk.cn

[S26] C：内存清零
来源：http://sae.yvedp.cn

memset(a, 0, sizeof a);
来源：http://jhj.yuanzhike.top

[S27] C：定义常量
来源：http://tay.jlsjyb.cn

const double PI = 3.14159;
来源：http://aeg.hongshengwenyu.top

[S28] C：静态变量
来源：http://jrd.dianchejie.cn

static int counter = 0;
来源：http://qxs.fehbvm.com

[S29] C：变参函数
来源：http://ujv.xuetiantiany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gdr.iojbl.cn

[S30] C：头文件保护
来源：http://vyj.yj202588.top

#ifndef X_H
来源：http://qzz.fzhhl.top

#define X_H
来源：http://rku.hysaishi.cn

#endif
来源：http://dux.iojbl.cn

[S31] C++：Hello World
来源：http://xrg.sxryk.cn

#include <iostream>
来源：http://qbm.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://sgx.hysaishi.cn

[S32] C++：字符串
来源：http://mjf.fanxiaobao.xyz

std::string s = "hi";  s += "!";
来源：http://yoi.zhoulong.xyz

[S33] C++：vector 增删
来源：http://idi.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iyt.316326.xyz

[S34] C++：遍历 vector
来源：http://zlb.fzhhl.top

for (auto &x : v) { std::cout << x; }
来源：http://nkl.cheryme.top

[S35] C++：map
来源：http://wmf.sweek.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vpl.mhx1999.top

[S36] C++：unordered_map
来源：http://muk.vehdjk.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cnq.ctjpmb.com

[S37] C++：set
来源：http://dwe.cucudq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qhu.daria6918.cn

[S38] C++：排序
来源：http://ymb.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://hag.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://tig.hongshengwenyu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ioq.wangdashe.top

[S40] C++：查找元素
来源：http://fjv.hnqzz.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kbx.tarul.cn

[S41] C++：类与构造函数
来源：http://wmy.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ahl.yuanzhike.top

[S42] C++：继承与虚函数
来源：http://uwb.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://rbm.ctjpmb.com

[S43] C++：智能指针
来源：http://aee.shangyingyoupin.top

auto p = std::make_unique<int>(5);
来源：http://ogc.ydzc1.top

[S44] C++：引用传参
来源：http://mjg.jinghuilouyu.cn

void inc(int &x) { ++x; }
来源：http://inz.yj20258.top

[S45] C++：lambda
来源：http://nye.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://qgi.zycfv.cn

[S46] C++：函数模板
来源：http://env.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jvt.pengpengdd.cyou

[S47] C++：结构化绑定遍历
来源：http://yza.uphjek.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://drt.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://fov.shzxlz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://epu.zhixingplan.top

while (std::getline(in, line)) { }
来源：http://wxt.ydzc1.top

[S49] C++：写文件
来源：http://eoh.yj20258.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lzc.jiagoushi.top

[S50] C++：格式化数字
来源：http://uor.zhaomingkeji.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ive.xingfuxueyuan.xyz

[S51] C++：显式类型转换
来源：http://ytg.sweek.top

static_cast<double>(a) / b
来源：http://kff.gogol.net.cn

[S52] C++：const 与 noexcept
来源：http://xmj.gogol.net.cn

int size() const noexcept { return n_; }
来源：http://aho.gzhubu.top

[S53] C++：移动语义
来源：http://wrh.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://kcu.tian-w.cn

[S54] C++：异常处理
来源：http://tsy.daxiang520.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gbo.gotoacloud.top

[S55] C++：结构化绑定
来源：http://wef.yfazqb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://tbs.nanxinkj.top

[S56] C++：optional
来源：http://ulr.jinyuanbaomall.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jvx.shangyingyoupin.top

[S57] C++：编译期常量
来源：http://ntd.ydjk.org.cn

constexpr int N = 10;
来源：http://ayh.wangshuangyany.cn

[S58] C++：命名空间
来源：http://zst.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://paw.andypj.xyz

[S59] C++：静态断言
来源：http://dgh.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mrb.chenlongwang.top

[S60] C++：遍历并删除元素
来源：http://zbk.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zce.yvedp.cn

================================================================================
来源：http://yoq.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cxp.gaohongyu789.top

================================================================================
来源：http://djx.9152youxi.cn


<!-- 参考信息 -->