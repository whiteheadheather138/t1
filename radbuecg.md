代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vwv.zdbjq.cn

[Q90] 生成序号列
来源：http://nwh.quarkkingdee.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rdn.fktsv.cn

================================================================================
来源：http://pxu.zhaomingkeji.xyz

R. Bash 专题
来源：http://tmb.gzhubu.top

================================================================================
来源：http://tyi.zhixingplan.top

[R01] shebang 与严格模式
来源：http://ymr.zhongyouzk.top

#!/usr/bin/env bash
来源：http://ard.guannengcc.top

set -euo pipefail
来源：http://qwg.316326.xyz

[R02] 变量赋值与使用
来源：http://qoe.xylfe.cn

name="Tom"; echo "$name"
来源：http://ffx.cqqwz.cn

[R03] 只读变量
来源：http://zdb.yuanzhike.top

readonly PI=3.14
来源：http://pvr.0kj1m.cn

[R04] 位置参数
来源：http://qgo.jyoumei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ekx.ehwqpu.com

[R05] 参数默认值
来源：http://lzd.gaohongyu789.top

name="${1:-default}"
来源：http://scu.yonumen.top

[R06] 判断命令是否存在
来源：http://kaz.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://faw.hcnkem.com

[R07] if 判断文件
来源：http://tya.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ydn.zhengqikj.top

[R08] 数值比较
来源：http://dpl.yvedp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ddt.bjfxy.top

[R09] 字符串比较
来源：http://ola.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oci.52xcode.cn

[R10] 正则匹配
来源：http://byy.ppjwa.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://owd.jlsjyb.cn

[R11] case 多分支
来源：http://gek.svipenyu.cn

case "$1" in
来源：http://iqj.sysykeji.top

start) echo "启动" ;;
来源：http://opt.guannengcc.top

stop)  echo "停止" ;;
来源：http://wwa.yonumen.top

*)     echo "未知命令" ;;
来源：http://lrs.nanxuanxn.top

esac
来源：http://mqd.yuanzhike.top

[R12] for 遍历文件
来源：http://qsf.tianlin.xyz

for f in *.txt; do echo "$f"; done
来源：http://qex.cheryme.top

[R13] for 计数循环
来源：http://nhl.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://uwr.316326.xyz

[R14] C 风格 for
来源：http://qjd.yangfankeji.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://urx.zhiwuduotai.top

[R15] while 逐行读文件
来源：http://jep.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pbz.jinghuilouyu.cn

[R16] until 等待条件
来源：http://mnt.zycfv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://adu.haohaochexian.top

[R17] 数组定义与取值
来源：http://udh.zhoulong.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://urs.fzhhl.top

[R18] 遍历数组
来源：http://ysy.ydzc1.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xzn.snrcjt.cn

[R19] 数组长度
来源：http://otw.gzhubu.top

echo "${#arr[@]}"
来源：http://ipj.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://yhb.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fbt.vqdsnc.cn

[R21] 字符串长度
来源：http://fwl.tian-w.cn

echo "${#s}"
来源：http://lts.hammf.cn

[R22] 截取子串
来源：http://xlo.mhx1999.top

echo "${s:0:5}"
来源：http://hhn.shanyushiyangtech.top

[R23] 字符串替换
来源：http://nmv.gzhubu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ndc.jqgfzy.top

[R24] 大小写转换
来源：http://owo.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://zoi.ppjwa.cn

[R25] 去后缀 / 去前缀
来源：http://cgw.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lsw.52xcode.cn

[R26] 命令替换
来源：http://jej.aizwys.cn

now=$(date +%F); echo "$now"
来源：http://wcj.meibo888.top

[R27] 算术展开
来源：http://wvq.zhongyouzk.top

echo $((1 + 2 * 3))
来源：http://noh.zhoulong.xyz

[R28] 浮点运算
来源：http://hqy.zhongyouzk.top

echo "scale=2; 10/3" | bc
来源：http://kld.xinyue.icu

[R29] 定义函数
来源：http://xox.ybcxt.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://chy.xuetiantiany.cn

[R30] 函数返回状态码
来源：http://cbt.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://cyf.nanxinkj.top

[R31] 局部变量
来源：http://bhd.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://rrw.tanke756.top

[R32] 参数个数校验
来源：http://xpg.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kmk.yueranfly.top

[R33] 捕获错误并提示行号
来源：http://meo.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dyx.jyoumei.cn

[R34] 退出时清理
来源：http://ava.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://oxv.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://ima.cdnleiting.top

sleep 5 & pid=$!; wait "$pid"
来源：http://err.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://vuu.chenzaomai.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oky.pengpengdd.cyou

[R37] 把输出赋给变量
来源：http://dtg.hongshengwenyu.top

files=$(ls -1)
来源：http://exc.xuetiantiany.cn

[R38] 管道串联
来源：http://gvf.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://xlw.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://eua.daria6918.cn

cmd > out.log 2>&1
来源：http://gzs.zhixingplan.top

[R40] 追加写日志
来源：http://glt.zhiwuduotai.top

echo "log" >> out.log
来源：http://qjb.sweek.top

[R41] 丢弃输出
来源：http://lpm.bbcook.cn

cmd >/dev/null 2>&1
来源：http://trx.hcnkem.com

[R42] 输入重定向
来源：http://kel.hnqzz.top

wc -l < a.txt
来源：http://hqy.guowangkeji.top

[R43] 按名字查找文件
来源：http://xaw.aizwys.cn

find . -name "*.log" -type f
来源：http://uiv.gotoacloud.top

[R44] 按修改时间查找
来源：http://szd.xinyue.icu

find . -mtime -7 -type f
来源：http://tmz.jinqigfzy.top

[R45] 批量删除
来源：http://sxr.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://urs.zycfv.cn

[R46] 递归替换文件内容
来源：http://lqs.xylfe.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qev.jianghu66.top

[R47] sed 单行替换
来源：http://bys.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://jsr.sxryk.cn

[R48] awk 取指定列
来源：http://swt.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://avy.yongpay.top

[R49] awk 带条件
来源：http://jol.shangyingyoupin.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dkh.fengsongda.top

[R50] awk 求和
来源：http://scm.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://bxg.tarul.cn

[R51] 排序去重取前几
来源：http://pgq.xziqi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bvh.316326.xyz

[R52] 统计行数
来源：http://cfr.xuanzx.com

wc -l a.txt
来源：http://jgh.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://unr.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nsy.sxryk.cn

[R54] 比较两个文件
来源：http://bsm.hfpthk.cn

diff a.txt b.txt
来源：http://rzt.gaohongyu789.top

[R55] 压缩与解压
来源：http://cro.xziqi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fso.yangfankeji.com

[R56] 远程拷贝
来源：http://omj.zhixingplan.top

scp file user@host:/path/
来源：http://mtw.cqqwz.cn

[R57] 远程执行命令
来源：http://wmj.sysykeji.top

ssh user@host 'uptime'
来源：http://mjm.hfpthk.cn

[R58] 下载文件
来源：http://wuf.zhengqikj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mrp.sweek.top

[R59] 发 POST JSON
来源：http://pri.jlsjyb.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uze.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://uvb.ctjpmb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uvb.yj20258.top

[R61] 磁盘占用
来源：http://kbl.mhx1999.top

df -h;  du -sh *
来源：http://cus.sxryk.cn

[R62] 找最占空间的文件
来源：http://ugm.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://eyu.ctjpmb.com

[R63] 内存与进程
来源：http://wdp.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://glz.nwbrower.top

[R64] 结束进程
来源：http://xge.316326.xyz

kill -9 $(pgrep -f app.py)
来源：http://sff.yfazqb.com

[R65] 查看端口占用
来源：http://hwu.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tgo.xuetiantiany.cn

[R66] 定时任务
来源：http://bxd.zycfv.cn

crontab -e;  crontab -l
来源：http://hlq.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://yei.vqdsnc.cn

openssl rand -hex 16
来源：http://jvq.yanxiufei.cn

[R68] 计算文件校验值
来源：http://ztz.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://xtv.smart0.xyz

[R69] 生成随机密码
来源：http://eho.nanxinkj.top

head -c 16 /dev/urandom | base64
来源：http://oaw.yj20258888.top

[R70] 时间戳与互转
来源：http://vtr.ehwqpu.com

date +%s;  date -d @1700000000
来源：http://obk.sufxvd.cn

[R71] 日期格式化
来源：http://dpp.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rwb.smart0.xyz

[R72] 等待端口就绪
来源：http://ocl.aizwys.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://btb.c1oappe.top

[R73] 分割大日志
来源：http://ger.chenlongwang.top

split -l 1000 big.log part_
来源：http://xvn.yongpay.top

[R74] 批量重命名
来源：http://npe.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ioi.zhijiandao.cn

[R75] 导出环境变量
来源：http://oxv.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://ugx.sweek.top

[R76] 使用临时文件
来源：http://vmx.jqgufenzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ooi.hysaishi.cn

[R77] 读取用户输入
来源：http://aut.yanxiufei.cn

read -rp "请输入: " ans
来源：http://brb.tanke756.top

[R78] 交互式菜单
来源：http://syw.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ilc.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://yud.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aea.ehwqpu.com

[R80] 查看脚本执行耗时
来源：http://acx.bjfxy.top

time ./run.sh
来源：http://qsk.tanke756.top

================================================================================
来源：http://bhg.shuidangran.top

S. C / C++ 专题
来源：http://hur.aibaodan.cn

================================================================================
来源：http://hyx.daxiang520.top

[S01] C：Hello World
来源：http://iix.316326.xyz

#include <stdio.h>
来源：http://uss.xuanzx.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://phk.cdnleiting.top

[S02] C：变量与格式化输出
来源：http://her.0kj1m.cn

int a = 10; printf("%d\n", a);
来源：http://lgx.haohaochexian.top

[S03] C：读入整数
来源：http://imj.ybcxt.top

int x; scanf("%d", &x);
来源：http://hzr.fengsongda.top

[S04] C：字符串复制
来源：http://kbc.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://wqz.fengsongda.top

[S05] C：字符串长度
来源：http://mva.vqdsnc.cn

strlen(s)
来源：http://snr.fehbvm.com

[S06] C：字符串比较
来源：http://kuq.316326.xyz

strcmp(a, b) == 0
来源：http://ucq.tianlin.xyz

[S07] C：数组遍历求和
来源：http://gvh.haohaochexian.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ltj.pengpengdd.cyou

[S08] C：动态内存分配与释放
来源：http://aee.xingfuxueyuan.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://umj.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://jii.zhixingplan.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ovf.316326.xyz

[S10] C：指针与解引用
来源：http://apk.sweek.top

int *p = &a;  *p = 5;
来源：http://cah.sjlbkw.cn

[S11] C：逐行读文件
来源：http://saz.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://elm.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rkm.yueranfly.top

fclose(f);
来源：http://tyj.tian-w.cn

[S12] C：写文件
来源：http://phx.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bgi.316326.xyz

[S13] C：宏定义
来源：http://sdu.yvedp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dkq.sweek.top

[S14] C：枚举
来源：http://dim.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://pfs.meibo888.top

[S15] C：类型转换
来源：http://iex.0kj1m.cn

(double) a / b
来源：http://mdo.0kj1m.cn

[S16] C：位操作置位
来源：http://uwj.zdqjudy.top

x |= (1 << 3);
来源：http://zzy.hnxiangtu.top

[S17] C：安全拼接字符串
来源：http://wgw.yj20258.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://stp.316326.xyz

[S18] C：命令行参数
来源：http://lcb.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://qnp.yj20258.top

[S19] C：快速排序
来源：http://ujz.ctjpmb.com

qsort(a, n, sizeof(int), cmp);
来源：http://yhi.gzhubu.top

[S20] C：二分查找
来源：http://csy.tianlin.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://plv.nwbrower.top

[S21] C：字符类别判断
来源：http://pqo.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qxc.gzhubu.top

[S22] C：字符串转数字
来源：http://cae.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://rqd.xuetiantiany.cn

[S23] C：随机数
来源：http://wdq.xuetiantiany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cdq.yuanzhike.top

[S24] C：获取本地时间
来源：http://mvm.jinqigfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jzw.yanxiufei.cn

[S25] C：内存拷贝
来源：http://unq.snrcjt.cn

memcpy(dst, src, n);
来源：http://ehx.xuanzx.com

[S26] C：内存清零
来源：http://jzm.jinghuilouyu.cn

memset(a, 0, sizeof a);
来源：http://isb.guannengcc.top

[S27] C：定义常量
来源：http://fmr.hcnkem.com

const double PI = 3.14159;
来源：http://jme.vehdjk.com

[S28] C：静态变量
来源：http://xzt.zycfv.cn

static int counter = 0;
来源：http://edj.jianghu66.top

[S29] C：变参函数
来源：http://wvb.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hou.yuxming.cn

[S30] C：头文件保护
来源：http://wgp.yueranfly.top

#ifndef X_H
来源：http://aft.sxryk.cn

#define X_H
来源：http://iba.yuanzhike.top

#endif
来源：http://evr.shzxlz.cn

[S31] C++：Hello World
来源：http://nnx.fanxiaobao.xyz

#include <iostream>
来源：http://uep.xinyue.icu

int main() { std::cout << "Hello\n"; }
来源：http://jic.cucudq.cn

[S32] C++：字符串
来源：http://sfn.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://bgs.sufxvd.cn

[S33] C++：vector 增删
来源：http://vrz.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cns.gogol.net.cn

[S34] C++：遍历 vector
来源：http://cpq.hysaishi.cn

for (auto &x : v) { std::cout << x; }
来源：http://ett.jyoumei.cn

[S35] C++：map
来源：http://ohu.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ddo.bbcook.cn

[S36] C++：unordered_map
来源：http://cow.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mxm.aibaodan.cn

[S37] C++：set
来源：http://lvj.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dam.9152youxi.cn

[S38] C++：排序
来源：http://ror.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://skm.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://uay.gaohongyu789.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rmi.tarul.cn

[S40] C++：查找元素
来源：http://sks.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zat.shuidangran.top

[S41] C++：类与构造函数
来源：http://znl.tianlin.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tda.fktsv.cn

[S42] C++：继承与虚函数
来源：http://kth.yj20258888.top

class B : public Base { public: void f() override {} };
来源：http://yxt.aizwys.cn

[S43] C++：智能指针
来源：http://isp.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://zgi.yuanzhike.top

[S44] C++：引用传参
来源：http://iee.cashguo.top

void inc(int &x) { ++x; }
来源：http://bjf.vehdjk.com

[S45] C++：lambda
来源：http://nyd.dianchejie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tll.cashguo.top

[S46] C++：函数模板
来源：http://esp.birdmap.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ywg.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://sqe.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dxl.ywan-chungtsiang.top

[S48] C++：逐行读文件
来源：http://lth.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://iqx.haohaochexian.top

while (std::getline(in, line)) { }
来源：http://ecl.yangfankeji.com

[S49] C++：写文件
来源：http://yeo.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ekd.hesvh.cn

[S50] C++：格式化数字
来源：http://sid.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://txv.guowangkeji.top

[S51] C++：显式类型转换
来源：http://xsn.nanxinkj.top

static_cast<double>(a) / b
来源：http://gnb.epnwcf.com

[S52] C++：const 与 noexcept
来源：http://lot.pycfn.com

int size() const noexcept { return n_; }
来源：http://mzj.shanyushiyangtech.top

[S53] C++：移动语义
来源：http://pkm.ybcxt.top

std::vector<int> w = std::move(v);
来源：http://xna.sxryk.cn

[S54] C++：异常处理
来源：http://qfy.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dms.yonumen.top

[S55] C++：结构化绑定
来源：http://thx.gotoacloud.top

auto [a, b] = std::make_pair(1, 2);
来源：http://epc.chenzaomai.com

[S56] C++：optional
来源：http://apo.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pid.sjlbkw.cn

[S57] C++：编译期常量
来源：http://ges.cheryme.top

constexpr int N = 10;
来源：http://qxp.zdbjq.cn

[S58] C++：命名空间
来源：http://bcs.pengpengdd.cyou

namespace ns { int f() { return 1; } }
来源：http://qfx.uphjek.com

[S59] C++：静态断言
来源：http://nzt.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rgz.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://djg.shanyushiyangtech.top


<!-- 参考信息 -->