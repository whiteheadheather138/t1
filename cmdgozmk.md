代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fjt.yuanzhike.top

[Q90] 生成序号列
来源：http://nyz.yonumen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://crg.ywan-chungtsiang.top

================================================================================
来源：http://nxu.guowangkeji.top

R. Bash 专题
来源：http://lic.xingfuxueyuan.xyz

================================================================================
来源：http://fqm.fanxiaobao.xyz

[R01] shebang 与严格模式
来源：http://cps.yj202588.top

#!/usr/bin/env bash
来源：http://zge.sxryk.cn

set -euo pipefail
来源：http://gtq.wangdashe.top

[R02] 变量赋值与使用
来源：http://avj.daria6918.cn

name="Tom"; echo "$name"
来源：http://dbi.0kj1m.cn

[R03] 只读变量
来源：http://pfi.quarkkingdee.top

readonly PI=3.14
来源：http://wpi.shanyushiyangtech.top

[R04] 位置参数
来源：http://epy.shzxlz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uac.jinqigfzy.top

[R05] 参数默认值
来源：http://hgc.fktsv.cn

name="${1:-default}"
来源：http://ocw.yueranfly.top

[R06] 判断命令是否存在
来源：http://yzt.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qbm.52xcode.cn

[R07] if 判断文件
来源：http://ubh.zhaomingkeji.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://erx.ydzc1.top

[R08] 数值比较
来源：http://rxp.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fhl.smart0.xyz

[R09] 字符串比较
来源：http://vij.zhixingplan.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kgy.jianghu66.top

[R10] 正则匹配
来源：http://fvx.sysykeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bmh.cucudq.cn

[R11] case 多分支
来源：http://hhh.jqgfzy.top

case "$1" in
来源：http://ush.yongpay.top

start) echo "启动" ;;
来源：http://ptv.jiagoushi.top

stop)  echo "停止" ;;
来源：http://zsx.fehbvm.com

*)     echo "未知命令" ;;
来源：http://bpv.hongshengwenyu.top

esac
来源：http://lzw.tarul.cn

[R12] for 遍历文件
来源：http://nuj.9152youxi.cn

for f in *.txt; do echo "$f"; done
来源：http://vdy.daria6918.cn

[R13] for 计数循环
来源：http://zmc.ydzc1.top

for i in {1..10}; do echo "$i"; done
来源：http://tyz.zhixingplan.top

[R14] C 风格 for
来源：http://qnl.yanxiufei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hlt.yonumen.top

[R15] while 逐行读文件
来源：http://bec.xingfuxueyuan.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tjw.havefunace.top

[R16] until 等待条件
来源：http://cwg.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tao.guowangkeji.top

[R17] 数组定义与取值
来源：http://rvh.yj202588.top

arr=(a b c); echo "${arr[0]}"
来源：http://rsy.tarul.cn

[R18] 遍历数组
来源：http://zyf.hcnkem.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wfa.epnwcf.com

[R19] 数组长度
来源：http://wpw.daxiang520.top

echo "${#arr[@]}"
来源：http://kjc.hysaishi.cn

[R20] 关联数组（字典）
来源：http://yub.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lcg.redwolf501.top

[R21] 字符串长度
来源：http://nci.hammf.cn

echo "${#s}"
来源：http://yfo.bbcook.cn

[R22] 截取子串
来源：http://rnc.pycfn.com

echo "${s:0:5}"
来源：http://kbm.ydzc1.top

[R23] 字符串替换
来源：http://sil.zhaomingkeji.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hme.redwolf501.top

[R24] 大小写转换
来源：http://bch.ybcxt.top

echo "${s^^}"; echo "${s,,}"
来源：http://utb.xingfuxueyuan.xyz

[R25] 去后缀 / 去前缀
来源：http://xmw.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eaw.xinyue.icu

[R26] 命令替换
来源：http://niw.meibo888.top

now=$(date +%F); echo "$now"
来源：http://ngg.yangfankeji.com

[R27] 算术展开
来源：http://yud.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://mro.gotoacloud.top

[R28] 浮点运算
来源：http://ddg.hesvh.cn

echo "scale=2; 10/3" | bc
来源：http://mhd.zhixingplan.top

[R29] 定义函数
来源：http://gbg.shanyushiyangtech.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yxu.havefunace.top

[R30] 函数返回状态码
来源：http://qqa.daxiang520.top

f() { return 0; }; f || echo "失败了"
来源：http://wcn.andypj.xyz

[R31] 局部变量
来源：http://ymg.jinyuanbaomall.cn

f() { local x=1; echo "$x"; }
来源：http://isj.hfpthk.cn

[R32] 参数个数校验
来源：http://sso.yanxiufei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nhr.hammf.cn

[R33] 捕获错误并提示行号
来源：http://seq.ctjpmb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jsp.feifeiyinyue.top

[R34] 退出时清理
来源：http://ssn.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://unl.yj20258.top

[R35] 后台执行并等待
来源：http://tro.fehbvm.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ipq.0kj1m.cn

[R36] 并发执行多个任务
来源：http://pex.52xcode.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ftn.yvedp.cn

[R37] 把输出赋给变量
来源：http://ifs.kuanghao11.cn

files=$(ls -1)
来源：http://ngk.sysykeji.top

[R38] 管道串联
来源：http://mje.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://tqv.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://qsl.gzhubu.top

cmd > out.log 2>&1
来源：http://qwy.yfazqb.com

[R40] 追加写日志
来源：http://rgy.fzhhl.top

echo "log" >> out.log
来源：http://ibo.shuidangran.top

[R41] 丢弃输出
来源：http://cdi.yueranfly.top

cmd >/dev/null 2>&1
来源：http://riz.havefunace.top

[R42] 输入重定向
来源：http://oxk.shuidangran.top

wc -l < a.txt
来源：http://krh.316326.xyz

[R43] 按名字查找文件
来源：http://tes.hysaishi.cn

find . -name "*.log" -type f
来源：http://ntv.jianghu66.top

[R44] 按修改时间查找
来源：http://odh.yueranfly.top

find . -mtime -7 -type f
来源：http://phd.daxiang520.top

[R45] 批量删除
来源：http://quo.tian-w.cn

find . -name "*.tmp" -delete
来源：http://cza.cqqwz.cn

[R46] 递归替换文件内容
来源：http://pui.wangshuangyany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uot.xylfe.cn

[R47] sed 单行替换
来源：http://fpe.xziqi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uii.havefunace.top

[R48] awk 取指定列
来源：http://kdm.tarul.cn

awk '{print $1, $3}' a.txt
来源：http://gzq.tarul.cn

[R49] awk 带条件
来源：http://nbu.snrcjt.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jkn.yueranfly.top

[R50] awk 求和
来源：http://twf.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://sxn.jianghu66.top

[R51] 排序去重取前几
来源：http://yur.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vsr.jinqigfzy.top

[R52] 统计行数
来源：http://qzg.jqgfzy.top

wc -l a.txt
来源：http://pra.hesvh.cn

[R53] 查看文件头与实时尾
来源：http://qoc.pengpengdd.cyou

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uqs.yangfankeji.com

[R54] 比较两个文件
来源：http://vxo.sweek.top

diff a.txt b.txt
来源：http://jtc.sjlbkw.cn

[R55] 压缩与解压
来源：http://ppl.gotoacloud.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bdt.hammf.cn

[R56] 远程拷贝
来源：http://mbe.havefunace.top

scp file user@host:/path/
来源：http://whu.aibaodan.cn

[R57] 远程执行命令
来源：http://pgx.kuanghao11.cn

ssh user@host 'uptime'
来源：http://zhs.nwbrower.top

[R58] 下载文件
来源：http://rpe.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://euj.cucudq.cn

[R59] 发 POST JSON
来源：http://kpc.bjfxy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tqy.yanxiufei.cn

[R60] 只看 HTTP 状态码
来源：http://shs.yj202588.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://apk.fzhhl.top

[R61] 磁盘占用
来源：http://fjj.yangfankeji.com

df -h;  du -sh *
来源：http://sjy.pengpengdd.cyou

[R62] 找最占空间的文件
来源：http://dtz.yongpay.top

du -ah . | sort -rh | head -10
来源：http://rug.jqgfzy.top

[R63] 内存与进程
来源：http://hvr.fanxiaobao.xyz

free -h;  ps aux | grep nginx
来源：http://iil.havefunace.top

[R64] 结束进程
来源：http://sif.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://upa.dashuyun.cn

[R65] 查看端口占用
来源：http://ybx.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gef.tarul.cn

[R66] 定时任务
来源：http://cys.haohaochexian.top

crontab -e;  crontab -l
来源：http://ygn.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://rfi.hcnkem.com

openssl rand -hex 16
来源：http://fvx.316326.xyz

[R68] 计算文件校验值
来源：http://ixr.yfazqb.com

sha256sum a.txt;  md5sum a.txt
来源：http://uce.fktsv.cn

[R69] 生成随机密码
来源：http://ldc.c1oappe.top

head -c 16 /dev/urandom | base64
来源：http://sqa.daxiang520.top

[R70] 时间戳与互转
来源：http://wgq.tian-w.cn

date +%s;  date -d @1700000000
来源：http://cxk.gotoacloud.top

[R71] 日期格式化
来源：http://rqk.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hch.pengpengdd.cyou

[R72] 等待端口就绪
来源：http://nym.yfazqb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://efi.zhengqikj.top

[R73] 分割大日志
来源：http://ezf.ywan-chungtsiang.top

split -l 1000 big.log part_
来源：http://bkt.chenzaomai.com

[R74] 批量重命名
来源：http://nmt.zhengqikj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ktq.chenlongwang.top

[R75] 导出环境变量
来源：http://guj.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://nsu.fanxiaobao.xyz

[R76] 使用临时文件
来源：http://omp.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://erp.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://hik.ctjpmb.com

read -rp "请输入: " ans
来源：http://fea.bjfxy.top

[R78] 交互式菜单
来源：http://krc.chenjidiqi.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://scc.dianchejie.cn

[R79] 解析命令行选项
来源：http://tkd.redwolf501.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fuz.hysaishi.cn

[R80] 查看脚本执行耗时
来源：http://xjc.vqdsnc.cn

time ./run.sh
来源：http://pwk.zhongyouzk.top

================================================================================
来源：http://wdn.feifeiyinyue.top

S. C / C++ 专题
来源：http://nyf.chenjidiqi.icu

================================================================================
来源：http://uxc.ydzc1.top

[S01] C：Hello World
来源：http://tnr.nanxuanxn.top

#include <stdio.h>
来源：http://rzt.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://psv.tianlin.xyz

[S02] C：变量与格式化输出
来源：http://tix.ywan-chungtsiang.top

int a = 10; printf("%d\n", a);
来源：http://fjk.andypj.xyz

[S03] C：读入整数
来源：http://yiu.c1oappe.top

int x; scanf("%d", &x);
来源：http://dzy.sweek.top

[S04] C：字符串复制
来源：http://ylz.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://eho.redwolf501.top

[S05] C：字符串长度
来源：http://ilg.wangshuangyany.cn

strlen(s)
来源：http://fhf.ehwqpu.com

[S06] C：字符串比较
来源：http://xji.zdqjudy.top

strcmp(a, b) == 0
来源：http://igc.yj20258888.top

[S07] C：数组遍历求和
来源：http://yff.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hex.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://rum.cheryme.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kyd.jinyuanbaomall.cn

[S09] C：结构体定义与初始化
来源：http://aba.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://frs.mhx1999.top

[S10] C：指针与解引用
来源：http://vct.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://zzl.fzhhl.top

[S11] C：逐行读文件
来源：http://ymi.zycfv.cn

FILE *f = fopen("a.txt", "r");
来源：http://znt.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wic.jianghu66.top

fclose(f);
来源：http://ikb.vehdjk.com

[S12] C：写文件
来源：http://cgu.kuanghao11.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cvp.hongshengwenyu.top

[S13] C：宏定义
来源：http://mma.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gyt.fanxiaobao.xyz

[S14] C：枚举
来源：http://rjm.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://ekc.shangyingyoupin.top

[S15] C：类型转换
来源：http://ahl.fehbvm.com

(double) a / b
来源：http://cuh.yuanzhike.top

[S16] C：位操作置位
来源：http://gob.sweek.top

x |= (1 << 3);
来源：http://ihz.wangdashe.top

[S17] C：安全拼接字符串
来源：http://tys.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://glf.nanxinkj.top

[S18] C：命令行参数
来源：http://wme.hywenlv.cn

int main(int argc, char **argv)
来源：http://dlu.vehdjk.com

[S19] C：快速排序
来源：http://fvv.hnqzz.top

qsort(a, n, sizeof(int), cmp);
来源：http://dvy.sysykeji.top

[S20] C：二分查找
来源：http://awm.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://thr.hammf.cn

[S21] C：字符类别判断
来源：http://skl.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rcx.sjlbkw.cn

[S22] C：字符串转数字
来源：http://wgb.jlsjyb.cn

atoi("42");  strtod("3.14", NULL);
来源：http://adl.birdmap.top

[S23] C：随机数
来源：http://xbh.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://bcj.aibaodan.cn

[S24] C：获取本地时间
来源：http://gez.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nwr.sxryk.cn

[S25] C：内存拷贝
来源：http://bwh.birdmap.top

memcpy(dst, src, n);
来源：http://gpt.cdnleiting.top

[S26] C：内存清零
来源：http://kvh.jianghu66.top

memset(a, 0, sizeof a);
来源：http://gwc.yj20258.top

[S27] C：定义常量
来源：http://qbj.cheryme.top

const double PI = 3.14159;
来源：http://bxi.bbcook.cn

[S28] C：静态变量
来源：http://osp.zhongyouzk.top

static int counter = 0;
来源：http://uwj.fzhhl.top

[S29] C：变参函数
来源：http://zsq.jqgufenzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gmz.yvedp.cn

[S30] C：头文件保护
来源：http://lto.zycfv.cn

#ifndef X_H
来源：http://pui.ydjk.org.cn

#define X_H
来源：http://vle.hammf.cn

#endif
来源：http://zvb.uphjek.com

[S31] C++：Hello World
来源：http://uuy.meibo888.top

#include <iostream>
来源：http://hew.cdnleiting.top

int main() { std::cout << "Hello\n"; }
来源：http://zua.gogol.net.cn

[S32] C++：字符串
来源：http://nkc.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://njd.jiagoushi.top

[S33] C++：vector 增删
来源：http://laf.cdnleiting.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nym.jinqigufen.top

[S34] C++：遍历 vector
来源：http://stz.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://imv.jinqigufen.top

[S35] C++：map
来源：http://hrq.zhengqikj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tnj.bjfxy.top

[S36] C++：unordered_map
来源：http://cuv.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mxx.fzhhl.top

[S37] C++：set
来源：http://arh.hesvh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mpj.0kj1m.cn

[S38] C++：排序
来源：http://joo.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://eel.jiagoushi.top

[S39] C++：自定义比较器排序
来源：http://yqj.gaohongyu789.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://syl.jiagoushi.top

[S40] C++：查找元素
来源：http://beu.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bfc.fzhhl.top

[S41] C++：类与构造函数
来源：http://uoj.zhijiandao.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://itv.yuanzhike.top

[S42] C++：继承与虚函数
来源：http://qib.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://veb.andypj.xyz

[S43] C++：智能指针
来源：http://rwj.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://yzd.316326.xyz

[S44] C++：引用传参
来源：http://tdf.yuxming.cn

void inc(int &x) { ++x; }
来源：http://jce.tanke756.top

[S45] C++：lambda
来源：http://iww.vqdsnc.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ovf.wangdashe.top

[S46] C++：函数模板
来源：http://nwy.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vpt.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://xew.havefunace.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ykw.mhx1999.top

[S48] C++：逐行读文件
来源：http://jot.9152youxi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lxa.aizwys.cn

while (std::getline(in, line)) { }
来源：http://aog.feifeiyinyue.top

[S49] C++：写文件
来源：http://ryc.zdqjudy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wtn.zycfv.cn

[S50] C++：格式化数字
来源：http://rwj.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lwc.cheryme.top

[S51] C++：显式类型转换
来源：http://kvp.yanxiufei.cn

static_cast<double>(a) / b
来源：http://tkq.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://sny.xziqi.cn

int size() const noexcept { return n_; }
来源：http://pqz.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://ifv.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://rgo.sxryk.cn

[S54] C++：异常处理
来源：http://vtw.hnxiangtu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mfw.hammf.cn

[S55] C++：结构化绑定
来源：http://qlp.yanxiufei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yyp.zdbjq.cn

[S56] C++：optional
来源：http://vpp.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sbz.hnxiangtu.top

[S57] C++：编译期常量
来源：http://zjn.hcnkem.com

constexpr int N = 10;
来源：http://mqw.cdnleiting.top

[S58] C++：命名空间
来源：http://tjh.zhijiandao.cn

namespace ns { int f() { return 1; } }
来源：http://yos.sjlbkw.cn

[S59] C++：静态断言
来源：http://gvh.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://egg.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://sjk.cqqwz.cn


<!-- 参考信息 -->