代发 wailian999

[Q86] 读取 JSON 字段
来源：http://jfa.xinyue.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zzz.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://qmk.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bxp.c1oappe.top

[Q88] 行转列（条件聚合）
来源：http://cud.fanxiaobao.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pgd.9152youxi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://exu.yonumen.top

[Q89] 判断表是否存在
来源：http://zpz.zycfv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://edl.gotoacloud.top

[Q90] 生成序号列
来源：http://pqn.bbcook.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ksf.quarkkingdee.top

================================================================================
来源：http://eto.yueranfly.top

R. Bash 专题
来源：http://ymf.jinqigfzy.top

================================================================================
来源：http://vec.chenzaomai.com

[R01] shebang 与严格模式
来源：http://udw.hnxiangtu.top

#!/usr/bin/env bash
来源：http://ejg.ywan-chungtsiang.top

set -euo pipefail
来源：http://rol.shanyushiyangkeji.top

[R02] 变量赋值与使用
来源：http://avu.quarkkingdee.top

name="Tom"; echo "$name"
来源：http://wgv.xingfuxueyuan.xyz

[R03] 只读变量
来源：http://tub.hcnkem.com

readonly PI=3.14
来源：http://mzj.jianghu66.top

[R04] 位置参数
来源：http://szy.shzxlz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cqp.hnqzz.top

[R05] 参数默认值
来源：http://odb.cucudq.cn

name="${1:-default}"
来源：http://gwy.shzxlz.cn

[R06] 判断命令是否存在
来源：http://vcs.ppjwa.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bzp.c1oappe.top

[R07] if 判断文件
来源：http://wka.zdqjudy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://usr.chenzaomai.com

[R08] 数值比较
来源：http://oul.kuanghao11.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vfa.yueranfly.top

[R09] 字符串比较
来源：http://sii.jinyuanbaomall.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://iis.zycfv.cn

[R10] 正则匹配
来源：http://ojq.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bwu.yj202588.top

[R11] case 多分支
来源：http://xyf.shanyushiyangtech.top

case "$1" in
来源：http://zba.ivvv.top

start) echo "启动" ;;
来源：http://kpo.gzhubu.top

stop)  echo "停止" ;;
来源：http://cjp.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://tlg.ybcxt.top

esac
来源：http://dvp.pycfn.com

[R12] for 遍历文件
来源：http://iib.andypj.xyz

for f in *.txt; do echo "$f"; done
来源：http://uyp.gogol.net.cn

[R13] for 计数循环
来源：http://nyv.yongpay.top

for i in {1..10}; do echo "$i"; done
来源：http://ygq.hcnkem.com

[R14] C 风格 for
来源：http://eqb.cqqwz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gao.xinyue.icu

[R15] while 逐行读文件
来源：http://usb.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ewg.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://iuz.jinghuilouyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jxz.tarul.cn

[R17] 数组定义与取值
来源：http://spv.smart0.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://jvd.uphjek.com

[R18] 遍历数组
来源：http://qmj.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zpb.cashguo.top

[R19] 数组长度
来源：http://vvf.ywan-chungtsiang.top

echo "${#arr[@]}"
来源：http://grk.zhiwuduotai.top

[R20] 关联数组（字典）
来源：http://ncm.0kj1m.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pep.snrcjt.cn

[R21] 字符串长度
来源：http://iip.jinqigfzy.top

echo "${#s}"
来源：http://eqt.hcnkem.com

[R22] 截取子串
来源：http://fwj.ydjk.org.cn

echo "${s:0:5}"
来源：http://ihs.52xcode.cn

[R23] 字符串替换
来源：http://osl.yongpay.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rqc.xylfe.cn

[R24] 大小写转换
来源：http://kpw.aibaodan.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bbx.dianchejie.cn

[R25] 去后缀 / 去前缀
来源：http://wbz.daria6918.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dtz.fzhhl.top

[R26] 命令替换
来源：http://ydm.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://qmg.vqdsnc.cn

[R27] 算术展开
来源：http://hxf.guannengcc.top

echo $((1 + 2 * 3))
来源：http://qrp.havefunace.top

[R28] 浮点运算
来源：http://fdw.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://llm.52xcode.cn

[R29] 定义函数
来源：http://rqe.vqdsnc.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uub.hnxiangtu.top

[R30] 函数返回状态码
来源：http://ycf.gogol.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://zdt.yangfankeji.com

[R31] 局部变量
来源：http://vri.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://lfw.yueranfly.top

[R32] 参数个数校验
来源：http://btr.pycfn.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ogs.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://xag.fanxiaobao.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xuq.yongpay.top

[R34] 退出时清理
来源：http://ier.smart0.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://spe.svipenyu.cn

[R35] 后台执行并等待
来源：http://qnj.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xag.jinyuanbaomall.cn

[R36] 并发执行多个任务
来源：http://azs.cucudq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wul.bjfxy.top

[R37] 把输出赋给变量
来源：http://yiu.svipenyu.cn

files=$(ls -1)
来源：http://pfy.gogol.net.cn

[R38] 管道串联
来源：http://vvq.fanxiaobao.xyz

cat a.txt | grep -i error | wc -l
来源：http://mjy.wangdashe.top

[R39] 重定向标准输出与错误
来源：http://oca.tianlin.xyz

cmd > out.log 2>&1
来源：http://ccf.shzxlz.cn

[R40] 追加写日志
来源：http://uwd.yj202588.top

echo "log" >> out.log
来源：http://ngu.svipenyu.cn

[R41] 丢弃输出
来源：http://wmx.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://nqe.birdmap.top

[R42] 输入重定向
来源：http://ipd.tanke756.top

wc -l < a.txt
来源：http://tmb.wangdashe.top

[R43] 按名字查找文件
来源：http://tbz.shzxlz.cn

find . -name "*.log" -type f
来源：http://ibs.zdqjudy.top

[R44] 按修改时间查找
来源：http://bzi.gzhubu.top

find . -mtime -7 -type f
来源：http://hxi.cheryme.top

[R45] 批量删除
来源：http://isg.hysaishi.cn

find . -name "*.tmp" -delete
来源：http://grv.daxiang520.top

[R46] 递归替换文件内容
来源：http://kls.dashuyun.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qcf.shuidangran.top

[R47] sed 单行替换
来源：http://sgu.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://gxp.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://qvh.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://nsa.hesvh.cn

[R49] awk 带条件
来源：http://jmf.jinqigufen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mqk.yfazqb.com

[R50] awk 求和
来源：http://qod.yongpay.top

awk '{s += $2} END {print s}' a.txt
来源：http://uae.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://rsx.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gue.xingfuxueyuan.xyz

[R52] 统计行数
来源：http://fmh.cheryme.top

wc -l a.txt
来源：http://fdq.hammf.cn

[R53] 查看文件头与实时尾
来源：http://djh.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ncw.nanxinkj.top

[R54] 比较两个文件
来源：http://syl.svipenyu.cn

diff a.txt b.txt
来源：http://jei.jyoumei.cn

[R55] 压缩与解压
来源：http://trs.yj202588.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xzi.tanke756.top

[R56] 远程拷贝
来源：http://lsi.hysaishi.cn

scp file user@host:/path/
来源：http://auf.yuanzhike.top

[R57] 远程执行命令
来源：http://cou.ivvv.top

ssh user@host 'uptime'
来源：http://dzm.hnqzz.top

[R58] 下载文件
来源：http://vpz.bjfxy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ouc.fanxiaobao.xyz

[R59] 发 POST JSON
来源：http://uba.ydjk.org.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dfi.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://jmm.xuanzx.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kvk.yj20258.top

[R61] 磁盘占用
来源：http://dzl.chenzaomai.com

df -h;  du -sh *
来源：http://gif.tianlin.xyz

[R62] 找最占空间的文件
来源：http://jtt.fehbvm.com

du -ah . | sort -rh | head -10
来源：http://cvg.bbcook.cn

[R63] 内存与进程
来源：http://yyq.pycfn.com

free -h;  ps aux | grep nginx
来源：http://soo.yueranfly.top

[R64] 结束进程
来源：http://tld.sweek.top

kill -9 $(pgrep -f app.py)
来源：http://gpc.hammf.cn

[R65] 查看端口占用
来源：http://lsa.bjfxy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://chf.ppjwa.cn

[R66] 定时任务
来源：http://zgk.xuanzx.com

crontab -e;  crontab -l
来源：http://zhr.sxryk.cn

[R67] 生成随机十六进制串
来源：http://aal.tianlin.xyz

openssl rand -hex 16
来源：http://hsh.guowangkeji.top

[R68] 计算文件校验值
来源：http://lbr.shanyushiyangtech.top

sha256sum a.txt;  md5sum a.txt
来源：http://qug.chenzaomai.com

[R69] 生成随机密码
来源：http://hkw.shuidangran.top

head -c 16 /dev/urandom | base64
来源：http://hny.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://pvm.nwbrower.top

date +%s;  date -d @1700000000
来源：http://lkv.nwbrower.top

[R71] 日期格式化
来源：http://oie.jinqigufen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wwy.sufxvd.cn

[R72] 等待端口就绪
来源：http://krt.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vdm.316326.xyz

[R73] 分割大日志
来源：http://abw.havefunace.top

split -l 1000 big.log part_
来源：http://mdh.hcnkem.com

[R74] 批量重命名
来源：http://sij.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fvk.redwolf501.top

[R75] 导出环境变量
来源：http://ayc.xingfuxueyuan.xyz

export PATH="$HOME/bin:$PATH"
来源：http://asx.ybcxt.top

[R76] 使用临时文件
来源：http://gei.cashguo.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zhn.kuanghao11.cn

[R77] 读取用户输入
来源：http://mzp.nanxinkj.top

read -rp "请输入: " ans
来源：http://neq.yvedp.cn

[R78] 交互式菜单
来源：http://lvu.pycfn.com

select opt in a b c; do echo "$opt"; break; done
来源：http://zut.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://ysu.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fdl.shzxlz.cn

[R80] 查看脚本执行耗时
来源：http://efp.fzhhl.top

time ./run.sh
来源：http://tkf.c1oappe.top

================================================================================
来源：http://rop.ehwqpu.com

S. C / C++ 专题
来源：http://zup.vehdjk.com

================================================================================
来源：http://rml.xuanzx.com

[S01] C：Hello World
来源：http://igb.snrcjt.cn

#include <stdio.h>
来源：http://vyq.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://giu.quarkkingdee.top

[S02] C：变量与格式化输出
来源：http://tim.pengpengdd.cyou

int a = 10; printf("%d\n", a);
来源：http://eed.jianghu66.top

[S03] C：读入整数
来源：http://wmu.xziqi.cn

int x; scanf("%d", &x);
来源：http://sls.shzxlz.cn

[S04] C：字符串复制
来源：http://egv.chenlongwang.top

char dst[32]; strcpy(dst, "hi");
来源：http://rsh.sufxvd.cn

[S05] C：字符串长度
来源：http://nwa.feifeiyinyue.top

strlen(s)
来源：http://akd.nwbrower.top

[S06] C：字符串比较
来源：http://gah.chenjidiqi.icu

strcmp(a, b) == 0
来源：http://zgs.vqdsnc.cn

[S07] C：数组遍历求和
来源：http://bej.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rsv.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://dem.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://npg.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://fec.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://una.yangfankeji.com

[S10] C：指针与解引用
来源：http://pch.epnwcf.com

int *p = &a;  *p = 5;
来源：http://phu.daria6918.cn

[S11] C：逐行读文件
来源：http://slz.aibaodan.cn

FILE *f = fopen("a.txt", "r");
来源：http://fuz.chenlongwang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pff.pengpengdd.cyou

fclose(f);
来源：http://xkt.dashuyun.cn

[S12] C：写文件
来源：http://fxk.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fbb.zhoulong.xyz

[S13] C：宏定义
来源：http://fct.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gco.jinyuanbaomall.cn

[S14] C：枚举
来源：http://aqu.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://ugy.sxryk.cn

[S15] C：类型转换
来源：http://vsc.guannengcc.top

(double) a / b
来源：http://edi.kuanghao11.cn

[S16] C：位操作置位
来源：http://mmr.shuidangran.top

x |= (1 << 3);
来源：http://nel.sxryk.cn

[S17] C：安全拼接字符串
来源：http://cvc.cheryme.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jlx.hcnkem.com

[S18] C：命令行参数
来源：http://vga.fanxiaobao.xyz

int main(int argc, char **argv)
来源：http://zqb.andypj.xyz

[S19] C：快速排序
来源：http://kwu.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://aww.yangfankeji.com

[S20] C：二分查找
来源：http://pgo.mhx1999.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kch.xziqi.cn

[S21] C：字符类别判断
来源：http://nxk.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cqg.cdnleiting.top

[S22] C：字符串转数字
来源：http://zip.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://nfz.ybcxt.top

[S23] C：随机数
来源：http://dcj.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ycj.feifeiyinyue.top

[S24] C：获取本地时间
来源：http://fbr.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nxm.shanyushiyangkeji.top

[S25] C：内存拷贝
来源：http://iyd.bjfxy.top

memcpy(dst, src, n);
来源：http://efe.zdqjudy.top

[S26] C：内存清零
来源：http://gvz.svipenyu.cn

memset(a, 0, sizeof a);
来源：http://dcp.316326.xyz

[S27] C：定义常量
来源：http://jdw.yongpay.top

const double PI = 3.14159;
来源：http://psj.gzhubu.top

[S28] C：静态变量
来源：http://ecq.kuanghao11.cn

static int counter = 0;
来源：http://dbj.shanyushiyangkeji.top

[S29] C：变参函数
来源：http://gyn.aizwys.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wpe.hongshengwenyu.top

[S30] C：头文件保护
来源：http://ipv.quarkkingdee.top

#ifndef X_H
来源：http://aym.shangyingyoupin.top

#define X_H
来源：http://cmt.yj202588.top

#endif
来源：http://zan.zdbjq.cn

[S31] C++：Hello World
来源：http://mko.gaohongyu789.top

#include <iostream>
来源：http://ohr.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://fiq.daria6918.cn

[S32] C++：字符串
来源：http://ayu.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://grb.hysaishi.cn

[S33] C++：vector 增删
来源：http://yoe.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qyw.hnqzz.top

[S34] C++：遍历 vector
来源：http://asw.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://qsd.chenlongwang.top

[S35] C++：map
来源：http://vrj.yuxming.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cvb.quarkkingdee.top

[S36] C++：unordered_map
来源：http://tle.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hlv.jinqigufen.top

[S37] C++：set
来源：http://kft.bbcook.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bje.sxryk.cn

[S38] C++：排序
来源：http://cun.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://tzv.cdnleiting.top

[S39] C++：自定义比较器排序
来源：http://orh.gaohongyu789.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ork.iojbl.cn

[S40] C++：查找元素
来源：http://add.sweek.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ybg.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://rwi.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uxx.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://jmp.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://kof.jinghuilouyu.cn

[S43] C++：智能指针
来源：http://jjp.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://kav.ywan-chungtsiang.top

[S44] C++：引用传参
来源：http://efb.fzhhl.top

void inc(int &x) { ++x; }
来源：http://oqx.haohaochexian.top

[S45] C++：lambda
来源：http://cks.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://xzb.guannengcc.top

[S46] C++：函数模板
来源：http://jhy.zhoulong.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xvq.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://uqi.yueranfly.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ulk.dianchejie.cn

[S48] C++：逐行读文件
来源：http://jfs.chenzaomai.com

std::ifstream in("a.txt");  std::string line;
来源：http://ntz.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://tpn.yueranfly.top

[S49] C++：写文件
来源：http://lrd.dashuyun.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gyr.daria6918.cn

[S50] C++：格式化数字
来源：http://qmd.shuidangran.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jxu.jianghu66.top

[S51] C++：显式类型转换
来源：http://vaf.jinqigufen.top

static_cast<double>(a) / b
来源：http://spg.hnqzz.top

[S52] C++：const 与 noexcept
来源：http://rmc.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://dnh.havefunace.top

[S53] C++：移动语义
来源：http://kvs.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://klp.jlsjyb.cn

[S54] C++：异常处理
来源：http://lag.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://itn.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://zht.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zot.xuanzx.com

[S56] C++：optional
来源：http://fwh.zhijiandao.cn


<!-- 参考信息 -->