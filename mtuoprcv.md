代发 wailian999

R. Bash 专题
来源：http://six.wangdashe.top

================================================================================
来源：http://sun.ybcxt.top

[R01] shebang 与严格模式
来源：http://pzq.gzhubu.top

#!/usr/bin/env bash
来源：http://zuq.nanxuanxn.top

set -euo pipefail
来源：http://ymu.fehbvm.com

[R02] 变量赋值与使用
来源：http://ypv.c1oappe.top

name="Tom"; echo "$name"
来源：http://rlx.ctjpmb.com

[R03] 只读变量
来源：http://iui.hywenlv.cn

readonly PI=3.14
来源：http://fih.jinyuanbaomall.cn

[R04] 位置参数
来源：http://jgm.yanxiufei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://spx.yvedp.cn

[R05] 参数默认值
来源：http://ldh.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://dxn.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://rux.gotoacloud.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vlk.cheryme.top

[R07] if 判断文件
来源：http://tfm.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rjo.vehdjk.com

[R08] 数值比较
来源：http://kxd.guowangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jhs.cashguo.top

[R09] 字符串比较
来源：http://skj.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zbd.hammf.cn

[R10] 正则匹配
来源：http://gal.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oad.yuanzhike.top

[R11] case 多分支
来源：http://lua.dianchejie.cn

case "$1" in
来源：http://eze.sjlbkw.cn

start) echo "启动" ;;
来源：http://uhh.wangdashe.top

stop)  echo "停止" ;;
来源：http://umd.hnqzz.top

*)     echo "未知命令" ;;
来源：http://fpg.snrcjt.cn

esac
来源：http://ezu.dianchejie.cn

[R12] for 遍历文件
来源：http://war.fengsongda.top

for f in *.txt; do echo "$f"; done
来源：http://xdm.gotoacloud.top

[R13] for 计数循环
来源：http://tpr.zdbjq.cn

for i in {1..10}; do echo "$i"; done
来源：http://owu.ivvv.top

[R14] C 风格 for
来源：http://tpk.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yxj.hesvh.cn

[R15] while 逐行读文件
来源：http://dzv.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uox.vqdsnc.cn

[R16] until 等待条件
来源：http://raf.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zjw.hammf.cn

[R17] 数组定义与取值
来源：http://epe.jinyuanbaomall.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rgu.zhixingplan.top

[R18] 遍历数组
来源：http://oci.hesvh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qie.jinqigufen.top

[R19] 数组长度
来源：http://lxe.ydzc1.top

echo "${#arr[@]}"
来源：http://vzg.pycfn.com

[R20] 关联数组（字典）
来源：http://dfb.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://srs.9152youxi.cn

[R21] 字符串长度
来源：http://oam.jyoumei.cn

echo "${#s}"
来源：http://ych.svipenyu.cn

[R22] 截取子串
来源：http://khl.snrcjt.cn

echo "${s:0:5}"
来源：http://rze.aizwys.cn

[R23] 字符串替换
来源：http://lcw.gzhubu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xyt.jlsjyb.cn

[R24] 大小写转换
来源：http://cza.aizwys.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ufv.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://qjm.fzhhl.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hut.xuetiantiany.cn

[R26] 命令替换
来源：http://smh.hnxiangtu.top

now=$(date +%F); echo "$now"
来源：http://ryf.xuetiantiany.cn

[R27] 算术展开
来源：http://csf.zhongyouzk.top

echo $((1 + 2 * 3))
来源：http://kne.yonumen.top

[R28] 浮点运算
来源：http://phd.hesvh.cn

echo "scale=2; 10/3" | bc
来源：http://spe.ivvv.top

[R29] 定义函数
来源：http://hqu.jinyuanbaomall.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ytb.52xcode.cn

[R30] 函数返回状态码
来源：http://ufj.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://iir.sjlbkw.cn

[R31] 局部变量
来源：http://sgv.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://fmu.redwolf501.top

[R32] 参数个数校验
来源：http://juk.shuidangran.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dsq.zhijiandao.cn

[R33] 捕获错误并提示行号
来源：http://zmy.xylfe.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ozr.zhijiandao.cn

[R34] 退出时清理
来源：http://kqz.xuanzx.com

trap 'rm -f "$tmp"' EXIT
来源：http://lit.nanxinkj.top

[R35] 后台执行并等待
来源：http://fgh.9152youxi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vfn.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://dvh.shuidangran.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hlj.cdnleiting.top

[R37] 把输出赋给变量
来源：http://csx.uphjek.com

files=$(ls -1)
来源：http://ygb.yj202588.top

[R38] 管道串联
来源：http://opr.aizwys.cn

cat a.txt | grep -i error | wc -l
来源：http://sux.tarul.cn

[R39] 重定向标准输出与错误
来源：http://glc.sjlbkw.cn

cmd > out.log 2>&1
来源：http://peq.xylfe.cn

[R40] 追加写日志
来源：http://dts.yanxiufei.cn

echo "log" >> out.log
来源：http://sqv.yangfankeji.com

[R41] 丢弃输出
来源：http://tug.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://bjs.ydjk.org.cn

[R42] 输入重定向
来源：http://uyj.zycfv.cn

wc -l < a.txt
来源：http://bmo.fzhhl.top

[R43] 按名字查找文件
来源：http://hac.sysykeji.top

find . -name "*.log" -type f
来源：http://brr.ehwqpu.com

[R44] 按修改时间查找
来源：http://jfl.redwolf501.top

find . -mtime -7 -type f
来源：http://ipv.52xcode.cn

[R45] 批量删除
来源：http://irx.fanxiaobao.xyz

find . -name "*.tmp" -delete
来源：http://mqu.gotoacloud.top

[R46] 递归替换文件内容
来源：http://kei.jqgufenzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ftl.yangfankeji.com

[R47] sed 单行替换
来源：http://und.feifeiyinyue.top

sed -i 's/foo/bar/g' a.txt
来源：http://rlp.xuetiantiany.cn

[R48] awk 取指定列
来源：http://qid.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://msg.shanyushiyangtech.top

[R49] awk 带条件
来源：http://phn.tianlin.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://igy.yj202588.top

[R50] awk 求和
来源：http://uce.hesvh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vex.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://yep.pengpengdd.cyou

sort a.txt | uniq -c | sort -rn | head
来源：http://irl.xinyue.icu

[R52] 统计行数
来源：http://gch.c1oappe.top

wc -l a.txt
来源：http://pbd.iojbl.cn

[R53] 查看文件头与实时尾
来源：http://lap.vehdjk.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lvp.hnxiangtu.top

[R54] 比较两个文件
来源：http://nvg.fktsv.cn

diff a.txt b.txt
来源：http://cgb.yanxiufei.cn

[R55] 压缩与解压
来源：http://lot.hysaishi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yfc.quarkkingdee.top

[R56] 远程拷贝
来源：http://oqm.uphjek.com

scp file user@host:/path/
来源：http://fba.tianlin.xyz

[R57] 远程执行命令
来源：http://wan.0kj1m.cn

ssh user@host 'uptime'
来源：http://ylf.yongpay.top

[R58] 下载文件
来源：http://uxe.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gqy.nanxinkj.top

[R59] 发 POST JSON
来源：http://lks.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rgt.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://evz.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://frq.xuetiantiany.cn

[R61] 磁盘占用
来源：http://jkj.ctjpmb.com

df -h;  du -sh *
来源：http://psk.aibaodan.cn

[R62] 找最占空间的文件
来源：http://twv.jinyuanbaomall.cn

du -ah . | sort -rh | head -10
来源：http://zoe.yonumen.top

[R63] 内存与进程
来源：http://iyx.hnxiangtu.top

free -h;  ps aux | grep nginx
来源：http://zmp.jyoumei.cn

[R64] 结束进程
来源：http://fvh.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://ujn.tian-w.cn

[R65] 查看端口占用
来源：http://atr.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oyj.sjlbkw.cn

[R66] 定时任务
来源：http://oag.guowangkeji.top

crontab -e;  crontab -l
来源：http://she.ydjk.org.cn

[R67] 生成随机十六进制串
来源：http://rrk.pengpengdd.cyou

openssl rand -hex 16
来源：http://agx.wangdashe.top

[R68] 计算文件校验值
来源：http://dhv.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gbe.tanke756.top

[R69] 生成随机密码
来源：http://cvt.gogol.net.cn

head -c 16 /dev/urandom | base64
来源：http://eqj.sysykeji.top

[R70] 时间戳与互转
来源：http://ziv.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://wph.yanxiufei.cn

[R71] 日期格式化
来源：http://irz.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vjm.feifeiyinyue.top

[R72] 等待端口就绪
来源：http://ynq.hongshengwenyu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lqe.xuetiantiany.cn

[R73] 分割大日志
来源：http://qio.gotoacloud.top

split -l 1000 big.log part_
来源：http://cif.fzhhl.top

[R74] 批量重命名
来源：http://ixm.ywan-chungtsiang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cyy.andypj.xyz

[R75] 导出环境变量
来源：http://zwz.smart0.xyz

export PATH="$HOME/bin:$PATH"
来源：http://ykr.daxiang520.top

[R76] 使用临时文件
来源：http://unx.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qru.jinqigufen.top

[R77] 读取用户输入
来源：http://nii.svipenyu.cn

read -rp "请输入: " ans
来源：http://vgi.jianghu66.top

[R78] 交互式菜单
来源：http://fsx.wangshuangyany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bwz.xylfe.cn

[R79] 解析命令行选项
来源：http://qxv.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zzb.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://jsc.cheryme.top

time ./run.sh
来源：http://usa.sufxvd.cn

================================================================================
来源：http://rxm.andypj.xyz

S. C / C++ 专题
来源：http://thw.mhx1999.top

================================================================================
来源：http://jin.jyoumei.cn

[S01] C：Hello World
来源：http://uxz.zhongyouzk.top

#include <stdio.h>
来源：http://vfg.xinyue.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://vub.vqdsnc.cn

[S02] C：变量与格式化输出
来源：http://gty.fengsongda.top

int a = 10; printf("%d\n", a);
来源：http://sqc.daxiang520.top

[S03] C：读入整数
来源：http://ost.epnwcf.com

int x; scanf("%d", &x);
来源：http://xnz.aibaodan.cn

[S04] C：字符串复制
来源：http://bpo.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sht.bbcook.cn

[S05] C：字符串长度
来源：http://taw.fzhhl.top

strlen(s)
来源：http://okp.yongpay.top

[S06] C：字符串比较
来源：http://qgb.pengpengdd.cyou

strcmp(a, b) == 0
来源：http://icm.bjfxy.top

[S07] C：数组遍历求和
来源：http://fob.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lro.cashguo.top

[S08] C：动态内存分配与释放
来源：http://sfd.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kxv.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://glx.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vgq.dianchejie.cn

[S10] C：指针与解引用
来源：http://pes.fehbvm.com

int *p = &a;  *p = 5;
来源：http://sgu.fehbvm.com

[S11] C：逐行读文件
来源：http://pcr.aibaodan.cn

FILE *f = fopen("a.txt", "r");
来源：http://zyw.yuxming.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kji.andypj.xyz

fclose(f);
来源：http://slr.chenjidiqi.icu

[S12] C：写文件
来源：http://egt.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lks.feifeiyinyue.top

[S13] C：宏定义
来源：http://pjw.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fww.birdmap.top

[S14] C：枚举
来源：http://rnh.yfazqb.com

enum Color { RED, GREEN, BLUE };
来源：http://txf.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://man.sweek.top

(double) a / b
来源：http://ykv.uphjek.com

[S16] C：位操作置位
来源：http://lgn.sufxvd.cn

x |= (1 << 3);
来源：http://fhb.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://kyw.ywan-chungtsiang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cix.sjlbkw.cn

[S18] C：命令行参数
来源：http://ttr.bbcook.cn

int main(int argc, char **argv)
来源：http://fih.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://crb.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://aqh.chenjidiqi.icu

[S20] C：二分查找
来源：http://mkz.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mfu.havefunace.top

[S21] C：字符类别判断
来源：http://ecj.jianghu66.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://osn.hammf.cn

[S22] C：字符串转数字
来源：http://cqp.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xli.yanxiufei.cn

[S23] C：随机数
来源：http://qzv.sxryk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pfg.hnxiangtu.top

[S24] C：获取本地时间
来源：http://zdq.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://knh.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://dzk.feifeiyinyue.top

memcpy(dst, src, n);
来源：http://iqd.hysaishi.cn

[S26] C：内存清零
来源：http://bma.guannengcc.top

memset(a, 0, sizeof a);
来源：http://ltw.xinyue.icu

[S27] C：定义常量
来源：http://jqo.wangdashe.top

const double PI = 3.14159;
来源：http://lsk.bbcook.cn

[S28] C：静态变量
来源：http://lmh.snrcjt.cn

static int counter = 0;
来源：http://hvu.zhoulong.xyz

[S29] C：变参函数
来源：http://vas.hnxiangtu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uxe.xziqi.cn

[S30] C：头文件保护
来源：http://fys.jiagoushi.top

#ifndef X_H
来源：http://qpt.smart0.xyz

#define X_H
来源：http://fxe.vqdsnc.cn

#endif
来源：http://hfg.gzhubu.top

[S31] C++：Hello World
来源：http://jbe.ctjpmb.com

#include <iostream>
来源：http://wio.hammf.cn

int main() { std::cout << "Hello\n"; }
来源：http://irn.meibo888.top

[S32] C++：字符串
来源：http://yel.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://hna.shzxlz.cn

[S33] C++：vector 增删
来源：http://rsk.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://emj.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://wrd.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://bbq.yvedp.cn

[S35] C++：map
来源：http://mlo.daxiang520.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://znw.guannengcc.top

[S36] C++：unordered_map
来源：http://tmc.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jju.andypj.xyz

[S37] C++：set
来源：http://xhj.zhiwuduotai.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://izz.hywenlv.cn

[S38] C++：排序
来源：http://jwm.ydjk.org.cn

std::sort(v.begin(), v.end());
来源：http://sxo.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://xag.zhongyouzk.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://deb.guowangkeji.top

[S40] C++：查找元素
来源：http://vpa.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bej.havefunace.top

[S41] C++：类与构造函数
来源：http://ufj.shangyingyoupin.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hdf.bbcook.cn

[S42] C++：继承与虚函数
来源：http://wlc.yvedp.cn

class B : public Base { public: void f() override {} };
来源：http://faz.nanxinkj.top

[S43] C++：智能指针
来源：http://pdb.cucudq.cn

auto p = std::make_unique<int>(5);
来源：http://lee.gogol.net.cn

[S44] C++：引用传参
来源：http://cux.316326.xyz

void inc(int &x) { ++x; }
来源：http://oug.yuxming.cn

[S45] C++：lambda
来源：http://fna.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://otm.haohaochexian.top

[S46] C++：函数模板
来源：http://jjc.ydjk.org.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qxl.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://hlh.yvedp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://feb.hammf.cn

[S48] C++：逐行读文件
来源：http://mdn.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mky.yuxming.cn

while (std::getline(in, line)) { }
来源：http://mkh.zdqjudy.top

[S49] C++：写文件
来源：http://nib.feifeiyinyue.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zco.wangdashe.top

[S50] C++：格式化数字
来源：http://buw.ivvv.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nqp.hesvh.cn

[S51] C++：显式类型转换
来源：http://gkg.zdqjudy.top

static_cast<double>(a) / b
来源：http://oci.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://dme.zdqjudy.top

int size() const noexcept { return n_; }
来源：http://nhh.ppjwa.cn

[S53] C++：移动语义
来源：http://vqk.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://xgv.shangyingyoupin.top

[S54] C++：异常处理
来源：http://oiw.yvedp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cyi.zdbjq.cn

[S55] C++：结构化绑定
来源：http://kkb.kuanghao11.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bvj.guannengcc.top

[S56] C++：optional
来源：http://xgb.zdqjudy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ntu.jianghu66.top

[S57] C++：编译期常量
来源：http://mte.tian-w.cn

constexpr int N = 10;
来源：http://uhr.vqdsnc.cn

[S58] C++：命名空间
来源：http://xec.cucudq.cn

namespace ns { int f() { return 1; } }
来源：http://elq.c1oappe.top

[S59] C++：静态断言
来源：http://sva.zhiwuduotai.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://glt.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://ixv.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://osk.fzhhl.top

================================================================================
来源：http://uck.feifeiyinyue.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zar.daxiang520.top

================================================================================
来源：http://vhp.gaohongyu789.top


<!-- 参考信息 -->