代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://chq.ivvv.top

[Q90] 生成序号列
来源：http://ivj.fktsv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xan.bbcook.cn

================================================================================
来源：http://hnu.hysaishi.cn

R. Bash 专题
来源：http://lni.cdnleiting.top

================================================================================
来源：http://jgl.wangdashe.top

[R01] shebang 与严格模式
来源：http://zbi.birdmap.top

#!/usr/bin/env bash
来源：http://ubq.zdbjq.cn

set -euo pipefail
来源：http://ivz.tarul.cn

[R02] 变量赋值与使用
来源：http://qyc.pengpengdd.cyou

name="Tom"; echo "$name"
来源：http://nnw.jinyuanbaomall.cn

[R03] 只读变量
来源：http://gms.fanxiaobao.xyz

readonly PI=3.14
来源：http://jut.jianghu66.top

[R04] 位置参数
来源：http://rdy.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://emx.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://isi.zhixingplan.top

name="${1:-default}"
来源：http://lew.cqqwz.cn

[R06] 判断命令是否存在
来源：http://awa.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ery.iojbl.cn

[R07] if 判断文件
来源：http://mpl.bjfxy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wjz.jiagoushi.top

[R08] 数值比较
来源：http://tys.ctjpmb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://xjv.yonumen.top

[R09] 字符串比较
来源：http://ydv.yonumen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://krr.cheryme.top

[R10] 正则匹配
来源：http://rtc.hcnkem.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://llh.yvedp.cn

[R11] case 多分支
来源：http://tqk.hysaishi.cn

case "$1" in
来源：http://uve.jlsjyb.cn

start) echo "启动" ;;
来源：http://dnj.zdqjudy.top

stop)  echo "停止" ;;
来源：http://npj.gaohongyu789.top

*)     echo "未知命令" ;;
来源：http://hzt.pengpengdd.cyou

esac
来源：http://rgm.tian-w.cn

[R12] for 遍历文件
来源：http://iaa.cheryme.top

for f in *.txt; do echo "$f"; done
来源：http://ant.ybcxt.top

[R13] for 计数循环
来源：http://pbg.zhengqikj.top

for i in {1..10}; do echo "$i"; done
来源：http://tqz.nanxuanxn.top

[R14] C 风格 for
来源：http://gkl.ywan-chungtsiang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uyp.jiagoushi.top

[R15] while 逐行读文件
来源：http://mls.yj20258.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sly.vehdjk.com

[R16] until 等待条件
来源：http://ldo.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cas.yanxiufei.cn

[R17] 数组定义与取值
来源：http://jsg.wangshuangyany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jgr.sufxvd.cn

[R18] 遍历数组
来源：http://efx.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rid.yj20258.top

[R19] 数组长度
来源：http://vjg.hfpthk.cn

echo "${#arr[@]}"
来源：http://cfs.ydjk.org.cn

[R20] 关联数组（字典）
来源：http://jyz.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wmm.ctjpmb.com

[R21] 字符串长度
来源：http://zdx.hnqzz.top

echo "${#s}"
来源：http://ezw.epnwcf.com

[R22] 截取子串
来源：http://fbh.zhixingplan.top

echo "${s:0:5}"
来源：http://vxq.bjfxy.top

[R23] 字符串替换
来源：http://cpd.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fbx.yfazqb.com

[R24] 大小写转换
来源：http://zfj.cdnleiting.top

echo "${s^^}"; echo "${s,,}"
来源：http://ylu.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://vth.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ffm.xingfuxueyuan.xyz

[R26] 命令替换
来源：http://cuv.cdnleiting.top

now=$(date +%F); echo "$now"
来源：http://tjl.iojbl.cn

[R27] 算术展开
来源：http://lul.nwbrower.top

echo $((1 + 2 * 3))
来源：http://cxn.redwolf501.top

[R28] 浮点运算
来源：http://wom.cucudq.cn

echo "scale=2; 10/3" | bc
来源：http://oll.xylfe.cn

[R29] 定义函数
来源：http://vom.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mls.yfazqb.com

[R30] 函数返回状态码
来源：http://mrt.xinyue.icu

f() { return 0; }; f || echo "失败了"
来源：http://xbd.dianchejie.cn

[R31] 局部变量
来源：http://hjm.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://suj.fehbvm.com

[R32] 参数个数校验
来源：http://fgq.zhoulong.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rfr.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://wya.xziqi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yms.feifeiyinyue.top

[R34] 退出时清理
来源：http://xow.gogol.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qqm.tian-w.cn

[R35] 后台执行并等待
来源：http://jgm.yuxming.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mpx.hcnkem.com

[R36] 并发执行多个任务
来源：http://utl.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://exj.uphjek.com

[R37] 把输出赋给变量
来源：http://mmc.yanxiufei.cn

files=$(ls -1)
来源：http://byk.shanyushiyangtech.top

[R38] 管道串联
来源：http://jut.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://ryc.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://uwp.shzxlz.cn

cmd > out.log 2>&1
来源：http://frr.0kj1m.cn

[R40] 追加写日志
来源：http://yzw.cucudq.cn

echo "log" >> out.log
来源：http://jse.bbcook.cn

[R41] 丢弃输出
来源：http://dbb.cqqwz.cn

cmd >/dev/null 2>&1
来源：http://big.wangshuangyany.cn

[R42] 输入重定向
来源：http://ohr.sjlbkw.cn

wc -l < a.txt
来源：http://fph.zycfv.cn

[R43] 按名字查找文件
来源：http://ljm.yuxming.cn

find . -name "*.log" -type f
来源：http://rev.uphjek.com

[R44] 按修改时间查找
来源：http://iqn.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://unb.gogol.net.cn

[R45] 批量删除
来源：http://acl.wangdashe.top

find . -name "*.tmp" -delete
来源：http://knd.xuanzx.com

[R46] 递归替换文件内容
来源：http://dnd.xinyue.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xqy.hcnkem.com

[R47] sed 单行替换
来源：http://lpr.yj20258.top

sed -i 's/foo/bar/g' a.txt
来源：http://uot.haohaochexian.top

[R48] awk 取指定列
来源：http://igv.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://nid.cucudq.cn

[R49] awk 带条件
来源：http://fzg.andypj.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pds.sweek.top

[R50] awk 求和
来源：http://iga.ywan-chungtsiang.top

awk '{s += $2} END {print s}' a.txt
来源：http://wdm.yuxming.cn

[R51] 排序去重取前几
来源：http://art.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dsk.nanxinkj.top

[R52] 统计行数
来源：http://mjd.sjlbkw.cn

wc -l a.txt
来源：http://ejm.xuetiantiany.cn

[R53] 查看文件头与实时尾
来源：http://gch.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rna.cucudq.cn

[R54] 比较两个文件
来源：http://cfw.ybcxt.top

diff a.txt b.txt
来源：http://mhc.yfazqb.com

[R55] 压缩与解压
来源：http://eir.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rli.hywenlv.cn

[R56] 远程拷贝
来源：http://alx.hywenlv.cn

scp file user@host:/path/
来源：http://ajf.epnwcf.com

[R57] 远程执行命令
来源：http://snz.9152youxi.cn

ssh user@host 'uptime'
来源：http://fki.yfazqb.com

[R58] 下载文件
来源：http://lub.hysaishi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://joo.zhengqikj.top

[R59] 发 POST JSON
来源：http://jsz.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zkd.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://uyh.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xab.zhixingplan.top

[R61] 磁盘占用
来源：http://sgf.zhongyouzk.top

df -h;  du -sh *
来源：http://aqg.birdmap.top

[R62] 找最占空间的文件
来源：http://lmq.tarul.cn

du -ah . | sort -rh | head -10
来源：http://frt.gotoacloud.top

[R63] 内存与进程
来源：http://kbr.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://ozs.nanxinkj.top

[R64] 结束进程
来源：http://jjs.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://qsx.uphjek.com

[R65] 查看端口占用
来源：http://pzo.shuidangran.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gbd.nwbrower.top

[R66] 定时任务
来源：http://giw.meibo888.top

crontab -e;  crontab -l
来源：http://udo.yongpay.top

[R67] 生成随机十六进制串
来源：http://aht.haohaochexian.top

openssl rand -hex 16
来源：http://ihu.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://tqu.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://tlb.xziqi.cn

[R69] 生成随机密码
来源：http://fua.ctjpmb.com

head -c 16 /dev/urandom | base64
来源：http://nnd.ywan-chungtsiang.top

[R70] 时间戳与互转
来源：http://shi.fzhhl.top

date +%s;  date -d @1700000000
来源：http://trt.aibaodan.cn

[R71] 日期格式化
来源：http://cwu.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eun.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://opt.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yls.chenjidiqi.icu

[R73] 分割大日志
来源：http://pwp.dashuyun.cn

split -l 1000 big.log part_
来源：http://jtg.dashuyun.cn

[R74] 批量重命名
来源：http://xrb.jyoumei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tse.cqqwz.cn

[R75] 导出环境变量
来源：http://tqb.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://wbz.52xcode.cn

[R76] 使用临时文件
来源：http://nvi.cashguo.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hpw.xziqi.cn

[R77] 读取用户输入
来源：http://cuz.gzhubu.top

read -rp "请输入: " ans
来源：http://ocg.redwolf501.top

[R78] 交互式菜单
来源：http://aob.bjfxy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://iro.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://zwa.hongshengwenyu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gas.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://mrh.hesvh.cn

time ./run.sh
来源：http://dnq.yueranfly.top

================================================================================
来源：http://cjd.birdmap.top

S. C / C++ 专题
来源：http://bpz.52xcode.cn

================================================================================
来源：http://bxr.0kj1m.cn

[S01] C：Hello World
来源：http://ful.uphjek.com

#include <stdio.h>
来源：http://yib.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jse.gaohongyu789.top

[S02] C：变量与格式化输出
来源：http://fri.52xcode.cn

int a = 10; printf("%d\n", a);
来源：http://yoj.meibo888.top

[S03] C：读入整数
来源：http://sow.guannengcc.top

int x; scanf("%d", &x);
来源：http://hxy.daria6918.cn

[S04] C：字符串复制
来源：http://hdw.xuetiantiany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rcx.gzhubu.top

[S05] C：字符串长度
来源：http://igy.yueranfly.top

strlen(s)
来源：http://ccv.ivvv.top

[S06] C：字符串比较
来源：http://tqc.jqgfzy.top

strcmp(a, b) == 0
来源：http://zml.0kj1m.cn

[S07] C：数组遍历求和
来源：http://scg.yj202588.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eoy.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://buj.vqdsnc.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dfo.shuidangran.top

[S09] C：结构体定义与初始化
来源：http://pbm.havefunace.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wbn.meibo888.top

[S10] C：指针与解引用
来源：http://jbx.hnqzz.top

int *p = &a;  *p = 5;
来源：http://jdz.yvedp.cn

[S11] C：逐行读文件
来源：http://egg.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://irb.hammf.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qme.redwolf501.top

fclose(f);
来源：http://vsy.havefunace.top

[S12] C：写文件
来源：http://tjr.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kmb.yuanzhike.top

[S13] C：宏定义
来源：http://eog.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nnl.meibo888.top

[S14] C：枚举
来源：http://bno.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://qvv.xylfe.cn

[S15] C：类型转换
来源：http://rkx.yonumen.top

(double) a / b
来源：http://bbs.vqdsnc.cn

[S16] C：位操作置位
来源：http://lwz.haohaochexian.top

x |= (1 << 3);
来源：http://bus.fengsongda.top

[S17] C：安全拼接字符串
来源：http://nxg.tanke756.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vfz.guannengcc.top

[S18] C：命令行参数
来源：http://eqr.sweek.top

int main(int argc, char **argv)
来源：http://nzd.hammf.cn

[S19] C：快速排序
来源：http://xmr.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://niz.jinghuilouyu.cn

[S20] C：二分查找
来源：http://yod.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jky.jinqigufen.top

[S21] C：字符类别判断
来源：http://xcq.xuetiantiany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bmo.jinyuanbaomall.cn

[S22] C：字符串转数字
来源：http://esg.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://tpf.hammf.cn

[S23] C：随机数
来源：http://fcs.zhongyouzk.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rxf.aibaodan.cn

[S24] C：获取本地时间
来源：http://noq.zycfv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ign.cashguo.top

[S25] C：内存拷贝
来源：http://obn.mhx1999.top

memcpy(dst, src, n);
来源：http://cra.hongshengwenyu.top

[S26] C：内存清零
来源：http://hul.vqdsnc.cn

memset(a, 0, sizeof a);
来源：http://kdq.316326.xyz

[S27] C：定义常量
来源：http://yin.birdmap.top

const double PI = 3.14159;
来源：http://jkg.ydjk.org.cn

[S28] C：静态变量
来源：http://gwq.yonumen.top

static int counter = 0;
来源：http://awh.zhaomingkeji.xyz

[S29] C：变参函数
来源：http://fqx.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jyu.yuxming.cn

[S30] C：头文件保护
来源：http://zxx.jinyuanbaomall.cn

#ifndef X_H
来源：http://pfb.xziqi.cn

#define X_H
来源：http://tjk.xuanzx.com

#endif
来源：http://rfi.aibaodan.cn

[S31] C++：Hello World
来源：http://fqb.zycfv.cn

#include <iostream>
来源：http://lqh.gzhubu.top

int main() { std::cout << "Hello\n"; }
来源：http://evd.ydzc1.top

[S32] C++：字符串
来源：http://xck.hcnkem.com

std::string s = "hi";  s += "!";
来源：http://vdh.jianghu66.top

[S33] C++：vector 增删
来源：http://maj.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wse.hammf.cn

[S34] C++：遍历 vector
来源：http://bkv.zdqjudy.top

for (auto &x : v) { std::cout << x; }
来源：http://xeb.zhiwuduotai.top

[S35] C++：map
来源：http://fbj.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jyo.dianchejie.cn

[S36] C++：unordered_map
来源：http://iza.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://roe.316326.xyz

[S37] C++：set
来源：http://toy.zdqjudy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hil.meibo888.top

[S38] C++：排序
来源：http://xdo.snrcjt.cn

std::sort(v.begin(), v.end());
来源：http://cuc.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://ice.yanxiufei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vsn.xuetiantiany.cn

[S40] C++：查找元素
来源：http://ywj.yueranfly.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bdf.yj202588.top

[S41] C++：类与构造函数
来源：http://get.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ypl.9152youxi.cn

[S42] C++：继承与虚函数
来源：http://fcm.9152youxi.cn

class B : public Base { public: void f() override {} };
来源：http://jhl.smart0.xyz

[S43] C++：智能指针
来源：http://ivh.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://cja.yj20258.top

[S44] C++：引用传参
来源：http://csg.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://end.ydzc1.top

[S45] C++：lambda
来源：http://rwo.guowangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://nxn.zhengqikj.top

[S46] C++：函数模板
来源：http://cdj.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wxu.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://nfb.yuxming.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fvv.jqgufenzy.top

[S48] C++：逐行读文件
来源：http://jnt.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://dek.cheryme.top

while (std::getline(in, line)) { }
来源：http://vyl.yj20258.top

[S49] C++：写文件
来源：http://dvh.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://usn.chenlongwang.top

[S50] C++：格式化数字
来源：http://cbp.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://knu.sxryk.cn

[S51] C++：显式类型转换
来源：http://qfd.0kj1m.cn

static_cast<double>(a) / b
来源：http://jad.tian-w.cn

[S52] C++：const 与 noexcept
来源：http://fqu.fktsv.cn

int size() const noexcept { return n_; }
来源：http://qkk.birdmap.top

[S53] C++：移动语义
来源：http://qkf.ehwqpu.com

std::vector<int> w = std::move(v);
来源：http://ziu.kuanghao11.cn

[S54] C++：异常处理
来源：http://ehn.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://exx.haohaochexian.top

[S55] C++：结构化绑定
来源：http://caq.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zuc.yonumen.top

[S56] C++：optional
来源：http://bou.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lrz.yj20258888.top

[S57] C++：编译期常量
来源：http://uti.haohaochexian.top

constexpr int N = 10;
来源：http://djv.epnwcf.com

[S58] C++：命名空间
来源：http://mnb.cdnleiting.top

namespace ns { int f() { return 1; } }
来源：http://jeq.svipenyu.cn

[S59] C++：静态断言
来源：http://btd.daxiang520.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://afw.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://bmg.sjlbkw.cn


<!-- 参考信息 -->