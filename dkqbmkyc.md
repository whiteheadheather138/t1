代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://eob.daxiang520.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://puv.fehbvm.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zfa.sufxvd.cn

[Q89] 判断表是否存在
来源：http://vob.yj20258888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xfk.yj20258.top

[Q90] 生成序号列
来源：http://xsy.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qpo.uphjek.com

================================================================================
来源：http://cfr.c1oappe.top

R. Bash 专题
来源：http://tpk.redwolf501.top

================================================================================
来源：http://jjq.dianchejie.cn

[R01] shebang 与严格模式
来源：http://zqa.xylfe.cn

#!/usr/bin/env bash
来源：http://sxf.xingfuxueyuan.xyz

set -euo pipefail
来源：http://jza.tanke756.top

[R02] 变量赋值与使用
来源：http://cbf.daria6918.cn

name="Tom"; echo "$name"
来源：http://dig.yangfankeji.com

[R03] 只读变量
来源：http://gpl.tanke756.top

readonly PI=3.14
来源：http://ecg.zhengqikj.top

[R04] 位置参数
来源：http://nqw.shanyushiyangtech.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dpz.sweek.top

[R05] 参数默认值
来源：http://uza.iojbl.cn

name="${1:-default}"
来源：http://uja.snrcjt.cn

[R06] 判断命令是否存在
来源：http://rfa.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://byb.xziqi.cn

[R07] if 判断文件
来源：http://xlg.c1oappe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://flm.nanxuanxn.top

[R08] 数值比较
来源：http://gjs.xylfe.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dft.cheryme.top

[R09] 字符串比较
来源：http://hxw.zhengqikj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xtw.xuanzx.com

[R10] 正则匹配
来源：http://ckp.quarkkingdee.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://faa.sxryk.cn

[R11] case 多分支
来源：http://kpb.hysaishi.cn

case "$1" in
来源：http://ckr.hysaishi.cn

start) echo "启动" ;;
来源：http://xwz.c1oappe.top

stop)  echo "停止" ;;
来源：http://ntw.cheryme.top

*)     echo "未知命令" ;;
来源：http://vsl.ydjk.org.cn

esac
来源：http://fuu.pycfn.com

[R12] for 遍历文件
来源：http://kwd.epnwcf.com

for f in *.txt; do echo "$f"; done
来源：http://fgf.hfpthk.cn

[R13] for 计数循环
来源：http://ppf.xingfuxueyuan.xyz

for i in {1..10}; do echo "$i"; done
来源：http://ogn.shzxlz.cn

[R14] C 风格 for
来源：http://bog.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qce.jinyuanbaomall.cn

[R15] while 逐行读文件
来源：http://mhv.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rlt.cucudq.cn

[R16] until 等待条件
来源：http://gki.chenlongwang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kjy.gogol.net.cn

[R17] 数组定义与取值
来源：http://bok.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://sqn.jlsjyb.cn

[R18] 遍历数组
来源：http://yil.ybcxt.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lbi.tian-w.cn

[R19] 数组长度
来源：http://tmq.chenlongwang.top

echo "${#arr[@]}"
来源：http://xht.hfpthk.cn

[R20] 关联数组（字典）
来源：http://dyi.yvedp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wim.iojbl.cn

[R21] 字符串长度
来源：http://xjk.yvedp.cn

echo "${#s}"
来源：http://dxh.ivvv.top

[R22] 截取子串
来源：http://mnq.9152youxi.cn

echo "${s:0:5}"
来源：http://hda.tarul.cn

[R23] 字符串替换
来源：http://nqi.hnqzz.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://piy.cheryme.top

[R24] 大小写转换
来源：http://fuj.epnwcf.com

echo "${s^^}"; echo "${s,,}"
来源：http://iti.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://exj.jinqigfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fqw.yj20258888.top

[R26] 命令替换
来源：http://fmo.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://ifd.dianchejie.cn

[R27] 算术展开
来源：http://xcq.meibo888.top

echo $((1 + 2 * 3))
来源：http://fwk.epnwcf.com

[R28] 浮点运算
来源：http://ytw.ybcxt.top

echo "scale=2; 10/3" | bc
来源：http://fqb.hnqzz.top

[R29] 定义函数
来源：http://yoh.dashuyun.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pkp.fzhhl.top

[R30] 函数返回状态码
来源：http://zac.andypj.xyz

f() { return 0; }; f || echo "失败了"
来源：http://dus.c1oappe.top

[R31] 局部变量
来源：http://elq.sxryk.cn

f() { local x=1; echo "$x"; }
来源：http://kqg.yueranfly.top

[R32] 参数个数校验
来源：http://frk.jinqigfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vvo.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://pvu.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mwc.zhengqikj.top

[R34] 退出时清理
来源：http://wel.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jna.jianghu66.top

[R35] 后台执行并等待
来源：http://pus.cucudq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zlh.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://wgs.fktsv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lny.tarul.cn

[R37] 把输出赋给变量
来源：http://dei.0kj1m.cn

files=$(ls -1)
来源：http://scm.c1oappe.top

[R38] 管道串联
来源：http://jqu.xuetiantiany.cn

cat a.txt | grep -i error | wc -l
来源：http://ysv.hnqzz.top

[R39] 重定向标准输出与错误
来源：http://pcd.redwolf501.top

cmd > out.log 2>&1
来源：http://rzq.cdnleiting.top

[R40] 追加写日志
来源：http://zsw.ydjk.org.cn

echo "log" >> out.log
来源：http://krz.jinqigfzy.top

[R41] 丢弃输出
来源：http://ukh.ydzc1.top

cmd >/dev/null 2>&1
来源：http://sxy.jqgufenzy.top

[R42] 输入重定向
来源：http://lwn.hcnkem.com

wc -l < a.txt
来源：http://ozp.ydzc1.top

[R43] 按名字查找文件
来源：http://ton.nwbrower.top

find . -name "*.log" -type f
来源：http://hmf.52xcode.cn

[R44] 按修改时间查找
来源：http://emh.jlsjyb.cn

find . -mtime -7 -type f
来源：http://itr.ydjk.org.cn

[R45] 批量删除
来源：http://kgw.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://dga.cashguo.top

[R46] 递归替换文件内容
来源：http://dkg.haohaochexian.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://amx.shuidangran.top

[R47] sed 单行替换
来源：http://nve.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://rlc.jinqigufen.top

[R48] awk 取指定列
来源：http://goi.yongpay.top

awk '{print $1, $3}' a.txt
来源：http://fzs.vqdsnc.cn

[R49] awk 带条件
来源：http://pxv.xziqi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cfe.daxiang520.top

[R50] awk 求和
来源：http://luf.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://jvm.yvedp.cn

[R51] 排序去重取前几
来源：http://jyn.tanke756.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bej.xingfuxueyuan.xyz

[R52] 统计行数
来源：http://hwi.zhengqikj.top

wc -l a.txt
来源：http://iyo.aizwys.cn

[R53] 查看文件头与实时尾
来源：http://wwv.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hla.mhx1999.top

[R54] 比较两个文件
来源：http://gla.ctjpmb.com

diff a.txt b.txt
来源：http://orq.andypj.xyz

[R55] 压缩与解压
来源：http://zkx.sysykeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vgy.yj20258888.top

[R56] 远程拷贝
来源：http://nrq.yueranfly.top

scp file user@host:/path/
来源：http://pva.hywenlv.cn

[R57] 远程执行命令
来源：http://tfn.chenlongwang.top

ssh user@host 'uptime'
来源：http://mle.redwolf501.top

[R58] 下载文件
来源：http://wse.yangfankeji.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nrh.yangfankeji.com

[R59] 发 POST JSON
来源：http://gtt.dianchejie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ugf.ybcxt.top

[R60] 只看 HTTP 状态码
来源：http://hxa.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nwl.jyoumei.cn

[R61] 磁盘占用
来源：http://gjk.zdbjq.cn

df -h;  du -sh *
来源：http://opv.0kj1m.cn

[R62] 找最占空间的文件
来源：http://fmc.jinyuanbaomall.cn

du -ah . | sort -rh | head -10
来源：http://ydk.ehwqpu.com

[R63] 内存与进程
来源：http://vbp.0kj1m.cn

free -h;  ps aux | grep nginx
来源：http://vpa.sufxvd.cn

[R64] 结束进程
来源：http://jgt.aizwys.cn

kill -9 $(pgrep -f app.py)
来源：http://yec.sysykeji.top

[R65] 查看端口占用
来源：http://ehr.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ywf.zhongyouzk.top

[R66] 定时任务
来源：http://kgr.jinqigfzy.top

crontab -e;  crontab -l
来源：http://ald.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://tpf.cucudq.cn

openssl rand -hex 16
来源：http://jcn.sxryk.cn

[R68] 计算文件校验值
来源：http://lxg.cdnleiting.top

sha256sum a.txt;  md5sum a.txt
来源：http://afb.jianghu66.top

[R69] 生成随机密码
来源：http://oby.hesvh.cn

head -c 16 /dev/urandom | base64
来源：http://gfe.bbcook.cn

[R70] 时间戳与互转
来源：http://aph.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://hga.haohaochexian.top

[R71] 日期格式化
来源：http://bvx.birdmap.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hxq.jianghu66.top

[R72] 等待端口就绪
来源：http://lpm.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jak.hfpthk.cn

[R73] 分割大日志
来源：http://hqy.xuanzx.com

split -l 1000 big.log part_
来源：http://fok.vqdsnc.cn

[R74] 批量重命名
来源：http://kmi.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hpy.ybcxt.top

[R75] 导出环境变量
来源：http://vlv.quarkkingdee.top

export PATH="$HOME/bin:$PATH"
来源：http://kcg.shangyingyoupin.top

[R76] 使用临时文件
来源：http://wvo.zhengqikj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ewk.aibaodan.cn

[R77] 读取用户输入
来源：http://udd.yfazqb.com

read -rp "请输入: " ans
来源：http://oyy.zycfv.cn

[R78] 交互式菜单
来源：http://tpo.quarkkingdee.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vrt.guannengcc.top

[R79] 解析命令行选项
来源：http://tnh.yangfankeji.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sep.sysykeji.top

[R80] 查看脚本执行耗时
来源：http://pwq.hnqzz.top

time ./run.sh
来源：http://ptq.bbcook.cn

================================================================================
来源：http://ohi.smart0.xyz

S. C / C++ 专题
来源：http://kte.ybcxt.top

================================================================================
来源：http://jvv.yj202588.top

[S01] C：Hello World
来源：http://qdz.gzhubu.top

#include <stdio.h>
来源：http://kyv.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://clj.yuanzhike.top

[S02] C：变量与格式化输出
来源：http://aor.jinghuilouyu.cn

int a = 10; printf("%d\n", a);
来源：http://gfv.vqdsnc.cn

[S03] C：读入整数
来源：http://djf.uphjek.com

int x; scanf("%d", &x);
来源：http://qiq.pengpengdd.cyou

[S04] C：字符串复制
来源：http://mxu.birdmap.top

char dst[32]; strcpy(dst, "hi");
来源：http://gsf.xziqi.cn

[S05] C：字符串长度
来源：http://kes.jinqigufen.top

strlen(s)
来源：http://kgw.gotoacloud.top

[S06] C：字符串比较
来源：http://apd.xinyue.icu

strcmp(a, b) == 0
来源：http://qzu.ppjwa.cn

[S07] C：数组遍历求和
来源：http://cxu.c1oappe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ayt.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://bdr.yj20258.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cia.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://rqt.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fkg.iojbl.cn

[S10] C：指针与解引用
来源：http://pvd.fehbvm.com

int *p = &a;  *p = 5;
来源：http://xup.hongshengwenyu.top

[S11] C：逐行读文件
来源：http://ron.hywenlv.cn

FILE *f = fopen("a.txt", "r");
来源：http://fwx.xinyue.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://vhi.zhixingplan.top

fclose(f);
来源：http://qos.yuanzhike.top

[S12] C：写文件
来源：http://bfl.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qab.yonumen.top

[S13] C：宏定义
来源：http://voz.yonumen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aqk.zhixingplan.top

[S14] C：枚举
来源：http://ibv.yvedp.cn

enum Color { RED, GREEN, BLUE };
来源：http://xfp.chenjidiqi.icu

[S15] C：类型转换
来源：http://pmr.wangshuangyany.cn

(double) a / b
来源：http://mbl.hnqzz.top

[S16] C：位操作置位
来源：http://rjo.uphjek.com

x |= (1 << 3);
来源：http://tzi.ctjpmb.com

[S17] C：安全拼接字符串
来源：http://wdu.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ffz.chenzaomai.com

[S18] C：命令行参数
来源：http://tdp.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://pks.dianchejie.cn

[S19] C：快速排序
来源：http://upe.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://xjm.nanxinkj.top

[S20] C：二分查找
来源：http://tcq.cdnleiting.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pgs.jianghu66.top

[S21] C：字符类别判断
来源：http://nuo.hammf.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vuv.0kj1m.cn

[S22] C：字符串转数字
来源：http://pji.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://yqd.xingfuxueyuan.xyz

[S23] C：随机数
来源：http://jhc.gotoacloud.top

srand(time(NULL));  int r = rand() % 100;
来源：http://crw.yvedp.cn

[S24] C：获取本地时间
来源：http://nhv.daria6918.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ibo.yangfankeji.com

[S25] C：内存拷贝
来源：http://gnj.bjfxy.top

memcpy(dst, src, n);
来源：http://wil.shuidangran.top

[S26] C：内存清零
来源：http://yjy.cqqwz.cn

memset(a, 0, sizeof a);
来源：http://xke.hongshengwenyu.top

[S27] C：定义常量
来源：http://vuc.jqgfzy.top

const double PI = 3.14159;
来源：http://abj.gzhubu.top

[S28] C：静态变量
来源：http://avv.zhongyouzk.top

static int counter = 0;
来源：http://uoj.kuanghao11.cn

[S29] C：变参函数
来源：http://joj.ydjk.org.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://scz.jqgfzy.top

[S30] C：头文件保护
来源：http://xxw.xinyue.icu

#ifndef X_H
来源：http://hau.cqqwz.cn

#define X_H
来源：http://rwz.shanyushiyangtech.top

#endif
来源：http://yjk.hysaishi.cn

[S31] C++：Hello World
来源：http://mpk.tianlin.xyz

#include <iostream>
来源：http://avj.zhijiandao.cn

int main() { std::cout << "Hello\n"; }
来源：http://wwh.jyoumei.cn

[S32] C++：字符串
来源：http://caz.hcnkem.com

std::string s = "hi";  s += "!";
来源：http://yng.hesvh.cn

[S33] C++：vector 增删
来源：http://vmh.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://axt.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://adg.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://sxi.fanxiaobao.xyz

[S35] C++：map
来源：http://dtt.zhengqikj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://spa.hnxiangtu.top

[S36] C++：unordered_map
来源：http://nnv.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ppd.xinyue.icu

[S37] C++：set
来源：http://jqu.chenjidiqi.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lle.aibaodan.cn

[S38] C++：排序
来源：http://nrj.uphjek.com

std::sort(v.begin(), v.end());
来源：http://qco.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://mke.zhengqikj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wkw.xziqi.cn

[S40] C++：查找元素
来源：http://ois.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rwp.316326.xyz

[S41] C++：类与构造函数
来源：http://tul.yonumen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wmn.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://wng.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://kms.wangshuangyany.cn

[S43] C++：智能指针
来源：http://wvw.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://fdx.yj202588.top

[S44] C++：引用传参
来源：http://jia.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://mkx.nwbrower.top

[S45] C++：lambda
来源：http://dnt.fanxiaobao.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://esq.shuidangran.top

[S46] C++：函数模板
来源：http://uhj.sjlbkw.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mwh.gogol.net.cn

[S47] C++：结构化绑定遍历
来源：http://frt.tian-w.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lnn.yfazqb.com

[S48] C++：逐行读文件
来源：http://egc.gaohongyu789.top

std::ifstream in("a.txt");  std::string line;
来源：http://yiu.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://ear.chenlongwang.top

[S49] C++：写文件
来源：http://mig.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uqq.wangshuangyany.cn

[S50] C++：格式化数字
来源：http://yzv.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zeg.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://whi.zdqjudy.top

static_cast<double>(a) / b
来源：http://ivc.shangyingyoupin.top

[S52] C++：const 与 noexcept
来源：http://rug.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://ykg.epnwcf.com

[S53] C++：移动语义
来源：http://kvg.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://cjd.zdbjq.cn

[S54] C++：异常处理
来源：http://qxr.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ibh.zhaomingkeji.xyz

[S55] C++：结构化绑定
来源：http://klq.sysykeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dxv.shanyushiyangtech.top

[S56] C++：optional
来源：http://mme.yj20258888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mod.ywan-chungtsiang.top

[S57] C++：编译期常量
来源：http://oua.jqgufenzy.top

constexpr int N = 10;
来源：http://mza.meibo888.top

[S58] C++：命名空间
来源：http://evd.xingfuxueyuan.xyz


<!-- 参考信息 -->