代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://nlb.cqqwz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://byt.xziqi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xrv.guowangkeji.top

[Q89] 判断表是否存在
来源：http://gxi.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vdq.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://pzi.guowangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iig.meibo888.top

================================================================================
来源：http://oue.tanke756.top

R. Bash 专题
来源：http://yaq.kuanghao11.cn

================================================================================
来源：http://pjs.yj20258888.top

[R01] shebang 与严格模式
来源：http://wbx.zdbjq.cn

#!/usr/bin/env bash
来源：http://mdm.haohaochexian.top

set -euo pipefail
来源：http://fuf.guowangkeji.top

[R02] 变量赋值与使用
来源：http://dcc.0kj1m.cn

name="Tom"; echo "$name"
来源：http://wno.shanyushiyangkeji.top

[R03] 只读变量
来源：http://vqg.wangdashe.top

readonly PI=3.14
来源：http://ytu.fzhhl.top

[R04] 位置参数
来源：http://qkr.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ywn.yonumen.top

[R05] 参数默认值
来源：http://gek.tanke756.top

name="${1:-default}"
来源：http://hxo.daxiang520.top

[R06] 判断命令是否存在
来源：http://jvq.zhiwuduotai.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://onq.zhaomingkeji.xyz

[R07] if 判断文件
来源：http://jjr.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vzi.yj202588.top

[R08] 数值比较
来源：http://tbf.cheryme.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zlw.aizwys.cn

[R09] 字符串比较
来源：http://xvy.yonumen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jsa.yuxming.cn

[R10] 正则匹配
来源：http://bys.cdnleiting.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zms.tian-w.cn

[R11] case 多分支
来源：http://prf.aizwys.cn

case "$1" in
来源：http://csc.wangdashe.top

start) echo "启动" ;;
来源：http://onk.cucudq.cn

stop)  echo "停止" ;;
来源：http://ijh.yonumen.top

*)     echo "未知命令" ;;
来源：http://kxb.zdbjq.cn

esac
来源：http://hwz.gogol.net.cn

[R12] for 遍历文件
来源：http://fkm.haohaochexian.top

for f in *.txt; do echo "$f"; done
来源：http://qgp.gotoacloud.top

[R13] for 计数循环
来源：http://jhh.52xcode.cn

for i in {1..10}; do echo "$i"; done
来源：http://nfl.guowangkeji.top

[R14] C 风格 for
来源：http://dxv.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sxe.hfpthk.cn

[R15] while 逐行读文件
来源：http://cwi.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qeg.daxiang520.top

[R16] until 等待条件
来源：http://ruo.dianchejie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fes.tanke756.top

[R17] 数组定义与取值
来源：http://sjb.cashguo.top

arr=(a b c); echo "${arr[0]}"
来源：http://hoa.gogol.net.cn

[R18] 遍历数组
来源：http://voo.sysykeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wic.hfpthk.cn

[R19] 数组长度
来源：http://fwj.sxryk.cn

echo "${#arr[@]}"
来源：http://njz.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://cau.zhixingplan.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jln.hnqzz.top

[R21] 字符串长度
来源：http://yuz.yvedp.cn

echo "${#s}"
来源：http://gak.nanxinkj.top

[R22] 截取子串
来源：http://tlb.quarkkingdee.top

echo "${s:0:5}"
来源：http://oud.hongshengwenyu.top

[R23] 字符串替换
来源：http://mlt.kuanghao11.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zsh.jianghu66.top

[R24] 大小写转换
来源：http://zzt.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jwl.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://eqb.jinyuanbaomall.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eix.wangdashe.top

[R26] 命令替换
来源：http://wre.jinghuilouyu.cn

now=$(date +%F); echo "$now"
来源：http://ndp.zhoulong.xyz

[R27] 算术展开
来源：http://gqg.vqdsnc.cn

echo $((1 + 2 * 3))
来源：http://mdz.snrcjt.cn

[R28] 浮点运算
来源：http://tmm.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://osy.pycfn.com

[R29] 定义函数
来源：http://tyt.xingfuxueyuan.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dbs.redwolf501.top

[R30] 函数返回状态码
来源：http://unc.vqdsnc.cn

f() { return 0; }; f || echo "失败了"
来源：http://wgx.ppjwa.cn

[R31] 局部变量
来源：http://epf.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://gqd.shzxlz.cn

[R32] 参数个数校验
来源：http://nbb.yj20258.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zag.fktsv.cn

[R33] 捕获错误并提示行号
来源：http://mav.hcnkem.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gpg.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://dyk.tarul.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cqf.birdmap.top

[R35] 后台执行并等待
来源：http://sqq.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://eco.zhengqikj.top

[R36] 并发执行多个任务
来源：http://azi.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gfe.nwbrower.top

[R37] 把输出赋给变量
来源：http://zwb.shuidangran.top

files=$(ls -1)
来源：http://ywe.aizwys.cn

[R38] 管道串联
来源：http://tij.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://zcm.chenlongwang.top

[R39] 重定向标准输出与错误
来源：http://msc.feifeiyinyue.top

cmd > out.log 2>&1
来源：http://oyn.tianlin.xyz

[R40] 追加写日志
来源：http://vhc.zhijiandao.cn

echo "log" >> out.log
来源：http://fnx.shanyushiyangtech.top

[R41] 丢弃输出
来源：http://koa.tian-w.cn

cmd >/dev/null 2>&1
来源：http://ita.0kj1m.cn

[R42] 输入重定向
来源：http://suw.xuetiantiany.cn

wc -l < a.txt
来源：http://dnw.haohaochexian.top

[R43] 按名字查找文件
来源：http://bgk.snrcjt.cn

find . -name "*.log" -type f
来源：http://mve.feifeiyinyue.top

[R44] 按修改时间查找
来源：http://pqy.zhijiandao.cn

find . -mtime -7 -type f
来源：http://taf.daxiang520.top

[R45] 批量删除
来源：http://xrv.dashuyun.cn

find . -name "*.tmp" -delete
来源：http://lnz.tian-w.cn

[R46] 递归替换文件内容
来源：http://mrh.zhiwuduotai.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pzq.jinyuanbaomall.cn

[R47] sed 单行替换
来源：http://klv.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://uhr.hnqzz.top

[R48] awk 取指定列
来源：http://gxc.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://rxy.jqgfzy.top

[R49] awk 带条件
来源：http://irj.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xwd.uphjek.com

[R50] awk 求和
来源：http://lbh.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ahh.haohaochexian.top

[R51] 排序去重取前几
来源：http://wvu.sweek.top

sort a.txt | uniq -c | sort -rn | head
来源：http://eql.hammf.cn

[R52] 统计行数
来源：http://juf.yongpay.top

wc -l a.txt
来源：http://xrh.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://vwj.havefunace.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://puz.ydjk.org.cn

[R54] 比较两个文件
来源：http://hnm.dianchejie.cn

diff a.txt b.txt
来源：http://fms.redwolf501.top

[R55] 压缩与解压
来源：http://xud.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://obe.cheryme.top

[R56] 远程拷贝
来源：http://auo.haohaochexian.top

scp file user@host:/path/
来源：http://wrm.havefunace.top

[R57] 远程执行命令
来源：http://qvr.zhixingplan.top

ssh user@host 'uptime'
来源：http://usc.zdbjq.cn

[R58] 下载文件
来源：http://jha.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tup.gogol.net.cn

[R59] 发 POST JSON
来源：http://loa.jinqigfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ikr.bjfxy.top

[R60] 只看 HTTP 状态码
来源：http://soe.chenlongwang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fpr.yvedp.cn

[R61] 磁盘占用
来源：http://hqq.aizwys.cn

df -h;  du -sh *
来源：http://owc.bjfxy.top

[R62] 找最占空间的文件
来源：http://jmp.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://sit.sweek.top

[R63] 内存与进程
来源：http://mnw.gogol.net.cn

free -h;  ps aux | grep nginx
来源：http://wfb.jqgufenzy.top

[R64] 结束进程
来源：http://nhe.aizwys.cn

kill -9 $(pgrep -f app.py)
来源：http://kid.0kj1m.cn

[R65] 查看端口占用
来源：http://uqf.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hoy.ybcxt.top

[R66] 定时任务
来源：http://ldr.svipenyu.cn

crontab -e;  crontab -l
来源：http://hub.nanxinkj.top

[R67] 生成随机十六进制串
来源：http://iyx.dianchejie.cn

openssl rand -hex 16
来源：http://vgw.svipenyu.cn

[R68] 计算文件校验值
来源：http://fsj.mhx1999.top

sha256sum a.txt;  md5sum a.txt
来源：http://nsm.dashuyun.cn

[R69] 生成随机密码
来源：http://qqc.yvedp.cn

head -c 16 /dev/urandom | base64
来源：http://jzd.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://pfc.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://jxs.kuanghao11.cn

[R71] 日期格式化
来源：http://pap.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kuj.fengsongda.top

[R72] 等待端口就绪
来源：http://ask.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xso.daria6918.cn

[R73] 分割大日志
来源：http://szg.dashuyun.cn

split -l 1000 big.log part_
来源：http://vyr.zycfv.cn

[R74] 批量重命名
来源：http://bti.52xcode.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qpo.ybcxt.top

[R75] 导出环境变量
来源：http://vyx.svipenyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://rld.aizwys.cn

[R76] 使用临时文件
来源：http://thp.quarkkingdee.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kka.nanxinkj.top

[R77] 读取用户输入
来源：http://sgs.snrcjt.cn

read -rp "请输入: " ans
来源：http://hwn.yueranfly.top

[R78] 交互式菜单
来源：http://vea.yvedp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dcf.fzhhl.top

[R79] 解析命令行选项
来源：http://fmo.hesvh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sfm.zycfv.cn

[R80] 查看脚本执行耗时
来源：http://thn.chenlongwang.top

time ./run.sh
来源：http://nps.jiagoushi.top

================================================================================
来源：http://gjg.cheryme.top

S. C / C++ 专题
来源：http://ymc.gogol.net.cn

================================================================================
来源：http://yxg.zhoulong.xyz

[S01] C：Hello World
来源：http://cmp.aizwys.cn

#include <stdio.h>
来源：http://fut.fengsongda.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kuz.jinghuilouyu.cn

[S02] C：变量与格式化输出
来源：http://muj.nanxuanxn.top

int a = 10; printf("%d\n", a);
来源：http://rmr.hesvh.cn

[S03] C：读入整数
来源：http://vwn.ivvv.top

int x; scanf("%d", &x);
来源：http://fad.hysaishi.cn

[S04] C：字符串复制
来源：http://ofa.xuetiantiany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ztl.jinqigufen.top

[S05] C：字符串长度
来源：http://uwc.aibaodan.cn

strlen(s)
来源：http://whp.yangfankeji.com

[S06] C：字符串比较
来源：http://www.hcnkem.com

strcmp(a, b) == 0
来源：http://uhf.chenlongwang.top

[S07] C：数组遍历求和
来源：http://tru.daria6918.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gtf.wangdashe.top

[S08] C：动态内存分配与释放
来源：http://rxg.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rwz.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://fqu.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gev.fzhhl.top

[S10] C：指针与解引用
来源：http://thz.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://liq.hongshengwenyu.top

[S11] C：逐行读文件
来源：http://jvq.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://gan.yj202588.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ryc.zhiwuduotai.top

fclose(f);
来源：http://kkf.zycfv.cn

[S12] C：写文件
来源：http://jnc.nanxinkj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mcu.cucudq.cn

[S13] C：宏定义
来源：http://pih.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jfa.tian-w.cn

[S14] C：枚举
来源：http://iox.hongshengwenyu.top

enum Color { RED, GREEN, BLUE };
来源：http://nbu.dianchejie.cn

[S15] C：类型转换
来源：http://cct.tianlin.xyz

(double) a / b
来源：http://oor.epnwcf.com

[S16] C：位操作置位
来源：http://rqu.nanxinkj.top

x |= (1 << 3);
来源：http://xaa.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://jky.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dkh.dianchejie.cn

[S18] C：命令行参数
来源：http://dbk.hcnkem.com

int main(int argc, char **argv)
来源：http://bjg.jinqigfzy.top

[S19] C：快速排序
来源：http://vij.wangshuangyany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://aqo.shanyushiyangkeji.top

[S20] C：二分查找
来源：http://csd.yj20258888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xrk.sjlbkw.cn

[S21] C：字符类别判断
来源：http://hvj.vehdjk.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oit.fengsongda.top

[S22] C：字符串转数字
来源：http://lxr.zhaomingkeji.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://ixi.shanyushiyangtech.top

[S23] C：随机数
来源：http://iht.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kyq.fktsv.cn

[S24] C：获取本地时间
来源：http://lob.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nxo.yanxiufei.cn

[S25] C：内存拷贝
来源：http://tur.havefunace.top

memcpy(dst, src, n);
来源：http://jux.hfpthk.cn

[S26] C：内存清零
来源：http://alw.cqqwz.cn

memset(a, 0, sizeof a);
来源：http://luz.zdbjq.cn

[S27] C：定义常量
来源：http://jqz.zhixingplan.top

const double PI = 3.14159;
来源：http://gnx.meibo888.top

[S28] C：静态变量
来源：http://vmu.jqgufenzy.top

static int counter = 0;
来源：http://mhq.yonumen.top

[S29] C：变参函数
来源：http://zao.gotoacloud.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://icg.jlsjyb.cn

[S30] C：头文件保护
来源：http://zhz.yvedp.cn

#ifndef X_H
来源：http://wxn.fzhhl.top

#define X_H
来源：http://qmo.xuanzx.com

#endif
来源：http://jik.vehdjk.com

[S31] C++：Hello World
来源：http://jbm.xuetiantiany.cn

#include <iostream>
来源：http://jko.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://zbv.havefunace.top

[S32] C++：字符串
来源：http://dyg.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://hec.yuanzhike.top

[S33] C++：vector 增删
来源：http://uwr.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://isx.yuxming.cn

[S34] C++：遍历 vector
来源：http://ddt.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://oss.tianlin.xyz

[S35] C++：map
来源：http://zvu.smart0.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eua.guannengcc.top

[S36] C++：unordered_map
来源：http://ngx.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nsb.snrcjt.cn

[S37] C++：set
来源：http://vuq.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ldb.fengsongda.top

[S38] C++：排序
来源：http://kmr.zhengqikj.top

std::sort(v.begin(), v.end());
来源：http://vxc.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://ikp.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cct.bjfxy.top

[S40] C++：查找元素
来源：http://eqf.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ewd.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://yen.nwbrower.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jla.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://ggr.mhx1999.top

class B : public Base { public: void f() override {} };
来源：http://olh.daria6918.cn

[S43] C++：智能指针
来源：http://ubk.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://cgj.sufxvd.cn

[S44] C++：引用传参
来源：http://fgp.hcnkem.com

void inc(int &x) { ++x; }
来源：http://wrf.dashuyun.cn

[S45] C++：lambda
来源：http://tsr.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://svk.hnxiangtu.top

[S46] C++：函数模板
来源：http://dmo.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zfs.hnqzz.top

[S47] C++：结构化绑定遍历
来源：http://hfy.316326.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ejw.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://xmo.shuidangran.top

std::ifstream in("a.txt");  std::string line;
来源：http://xbk.chenzaomai.com

while (std::getline(in, line)) { }
来源：http://lzi.aibaodan.cn

[S49] C++：写文件
来源：http://llu.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vol.nwbrower.top

[S50] C++：格式化数字
来源：http://uxl.yueranfly.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jnj.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://iey.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://tli.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://rtd.c1oappe.top

int size() const noexcept { return n_; }
来源：http://jsa.sxryk.cn

[S53] C++：移动语义
来源：http://rmm.0kj1m.cn

std::vector<int> w = std::move(v);
来源：http://pwr.zhixingplan.top

[S54] C++：异常处理
来源：http://dhh.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ruv.epnwcf.com

[S55] C++：结构化绑定
来源：http://xti.wangshuangyany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sye.wangshuangyany.cn

[S56] C++：optional
来源：http://fdm.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mvt.daxiang520.top

[S57] C++：编译期常量
来源：http://npz.wangshuangyany.cn

constexpr int N = 10;
来源：http://izn.jinqigufen.top

[S58] C++：命名空间
来源：http://ixv.chenzaomai.com


<!-- 参考信息 -->