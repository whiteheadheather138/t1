代发 wailian999

[Q84] 去除首尾空格
来源：http://iez.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://etg.cucudq.cn

[Q85] 数值取整
来源：http://tju.zhixingplan.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://luj.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://ycp.sxryk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lob.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://wcs.cheryme.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nsr.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://nog.guannengcc.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://arx.sxryk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vls.tarul.cn

[Q89] 判断表是否存在
来源：http://ifj.hywenlv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jhk.yfazqb.com

[Q90] 生成序号列
来源：http://wuk.jinqigufen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hye.bjfxy.top

================================================================================
来源：http://bbe.ctjpmb.com

R. Bash 专题
来源：http://ldv.jlsjyb.cn

================================================================================
来源：http://usb.gaohongyu789.top

[R01] shebang 与严格模式
来源：http://ohx.andypj.xyz

#!/usr/bin/env bash
来源：http://sxx.jinqigufen.top

set -euo pipefail
来源：http://vgm.havefunace.top

[R02] 变量赋值与使用
来源：http://lqc.ctjpmb.com

name="Tom"; echo "$name"
来源：http://wvk.zhaomingkeji.xyz

[R03] 只读变量
来源：http://sib.jinghuilouyu.cn

readonly PI=3.14
来源：http://oer.jiagoushi.top

[R04] 位置参数
来源：http://sej.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fvz.guannengcc.top

[R05] 参数默认值
来源：http://crd.fanxiaobao.xyz

name="${1:-default}"
来源：http://soh.hnqzz.top

[R06] 判断命令是否存在
来源：http://moa.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://irf.zhongyouzk.top

[R07] if 判断文件
来源：http://yrc.hywenlv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jhc.ybcxt.top

[R08] 数值比较
来源：http://cfy.guowangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bfx.nanxuanxn.top

[R09] 字符串比较
来源：http://bqq.ehwqpu.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rox.cdnleiting.top

[R10] 正则匹配
来源：http://oca.hysaishi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vhv.yj202588.top

[R11] case 多分支
来源：http://kgs.jiagoushi.top

case "$1" in
来源：http://fha.aibaodan.cn

start) echo "启动" ;;
来源：http://btu.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://qxu.epnwcf.com

*)     echo "未知命令" ;;
来源：http://vny.wangdashe.top

esac
来源：http://umw.chenzaomai.com

[R12] for 遍历文件
来源：http://twr.hammf.cn

for f in *.txt; do echo "$f"; done
来源：http://xay.fktsv.cn

[R13] for 计数循环
来源：http://utg.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://xho.kuanghao11.cn

[R14] C 风格 for
来源：http://nwg.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://esu.jqgufenzy.top

[R15] while 逐行读文件
来源：http://ttk.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ipf.shzxlz.cn

[R16] until 等待条件
来源：http://xod.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vax.uphjek.com

[R17] 数组定义与取值
来源：http://ify.gotoacloud.top

arr=(a b c); echo "${arr[0]}"
来源：http://ozb.kuanghao11.cn

[R18] 遍历数组
来源：http://bdf.yuanzhike.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qip.zhixingplan.top

[R19] 数组长度
来源：http://wbw.jiagoushi.top

echo "${#arr[@]}"
来源：http://bnx.zhoulong.xyz

[R20] 关联数组（字典）
来源：http://idp.hammf.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ucz.guowangkeji.top

[R21] 字符串长度
来源：http://yck.jianghu66.top

echo "${#s}"
来源：http://ops.shanyushiyangkeji.top

[R22] 截取子串
来源：http://hea.xinyue.icu

echo "${s:0:5}"
来源：http://ddb.c1oappe.top

[R23] 字符串替换
来源：http://ykk.ydjk.org.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lkc.zhijiandao.cn

[R24] 大小写转换
来源：http://twr.gogol.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hsa.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://sqp.hnxiangtu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lyc.c1oappe.top

[R26] 命令替换
来源：http://kzq.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://dnd.yvedp.cn

[R27] 算术展开
来源：http://xnt.andypj.xyz

echo $((1 + 2 * 3))
来源：http://gki.bjfxy.top

[R28] 浮点运算
来源：http://clg.zhaomingkeji.xyz

echo "scale=2; 10/3" | bc
来源：http://wpc.shuidangran.top

[R29] 定义函数
来源：http://unf.yongpay.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cgh.jiagoushi.top

[R30] 函数返回状态码
来源：http://vcc.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://bnb.pycfn.com

[R31] 局部变量
来源：http://wbp.ctjpmb.com

f() { local x=1; echo "$x"; }
来源：http://moj.cucudq.cn

[R32] 参数个数校验
来源：http://kxe.smart0.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vhm.ivvv.top

[R33] 捕获错误并提示行号
来源：http://jcr.cashguo.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xah.hysaishi.cn

[R34] 退出时清理
来源：http://uxh.jqgfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://znw.xylfe.cn

[R35] 后台执行并等待
来源：http://smr.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://sip.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://wbw.hfpthk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gdz.sweek.top

[R37] 把输出赋给变量
来源：http://aly.ybcxt.top

files=$(ls -1)
来源：http://kzk.iojbl.cn

[R38] 管道串联
来源：http://zzq.sweek.top

cat a.txt | grep -i error | wc -l
来源：http://syh.yj202588.top

[R39] 重定向标准输出与错误
来源：http://wvk.jqgfzy.top

cmd > out.log 2>&1
来源：http://msx.ydjk.org.cn

[R40] 追加写日志
来源：http://lis.pycfn.com

echo "log" >> out.log
来源：http://wvp.9152youxi.cn

[R41] 丢弃输出
来源：http://fky.zhongyouzk.top

cmd >/dev/null 2>&1
来源：http://uag.cucudq.cn

[R42] 输入重定向
来源：http://qcp.yj20258888.top

wc -l < a.txt
来源：http://qgz.xylfe.cn

[R43] 按名字查找文件
来源：http://qof.nwbrower.top

find . -name "*.log" -type f
来源：http://mud.gogol.net.cn

[R44] 按修改时间查找
来源：http://igj.vehdjk.com

find . -mtime -7 -type f
来源：http://vpj.nwbrower.top

[R45] 批量删除
来源：http://ret.fktsv.cn

find . -name "*.tmp" -delete
来源：http://xfh.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://voe.fzhhl.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lab.xylfe.cn

[R47] sed 单行替换
来源：http://thy.shuidangran.top

sed -i 's/foo/bar/g' a.txt
来源：http://bhp.zdqjudy.top

[R48] awk 取指定列
来源：http://ais.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://tsi.jyoumei.cn

[R49] awk 带条件
来源：http://ddx.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ipc.cashguo.top

[R50] awk 求和
来源：http://iwc.cashguo.top

awk '{s += $2} END {print s}' a.txt
来源：http://plb.jqgfzy.top

[R51] 排序去重取前几
来源：http://hje.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vxv.jlsjyb.cn

[R52] 统计行数
来源：http://hod.hcnkem.com

wc -l a.txt
来源：http://sux.pycfn.com

[R53] 查看文件头与实时尾
来源：http://gfb.birdmap.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gqd.yuxming.cn

[R54] 比较两个文件
来源：http://vng.haohaochexian.top

diff a.txt b.txt
来源：http://nsm.chenjidiqi.icu

[R55] 压缩与解压
来源：http://lji.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kpa.xinyue.icu

[R56] 远程拷贝
来源：http://mlt.hesvh.cn

scp file user@host:/path/
来源：http://uhi.svipenyu.cn

[R57] 远程执行命令
来源：http://jwk.yangfankeji.com

ssh user@host 'uptime'
来源：http://pyo.yangfankeji.com

[R58] 下载文件
来源：http://lmb.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ovr.jinghuilouyu.cn

[R59] 发 POST JSON
来源：http://vln.cashguo.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ibl.bjfxy.top

[R60] 只看 HTTP 状态码
来源：http://onx.sjlbkw.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jvs.hysaishi.cn

[R61] 磁盘占用
来源：http://jdw.xuanzx.com

df -h;  du -sh *
来源：http://pvb.cdnleiting.top

[R62] 找最占空间的文件
来源：http://mjj.vehdjk.com

du -ah . | sort -rh | head -10
来源：http://wot.gogol.net.cn

[R63] 内存与进程
来源：http://tik.hammf.cn

free -h;  ps aux | grep nginx
来源：http://wqf.feifeiyinyue.top

[R64] 结束进程
来源：http://tyx.quarkkingdee.top

kill -9 $(pgrep -f app.py)
来源：http://pff.jlsjyb.cn

[R65] 查看端口占用
来源：http://oqv.sxryk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fbw.gogol.net.cn

[R66] 定时任务
来源：http://txl.jinqigfzy.top

crontab -e;  crontab -l
来源：http://suu.xinyue.icu

[R67] 生成随机十六进制串
来源：http://rkl.sweek.top

openssl rand -hex 16
来源：http://ysc.havefunace.top

[R68] 计算文件校验值
来源：http://nyz.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://flc.hfpthk.cn

[R69] 生成随机密码
来源：http://uaw.xuanzx.com

head -c 16 /dev/urandom | base64
来源：http://nqe.yvedp.cn

[R70] 时间戳与互转
来源：http://zso.aizwys.cn

date +%s;  date -d @1700000000
来源：http://slz.wangdashe.top

[R71] 日期格式化
来源：http://oov.yueranfly.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zpc.jinghuilouyu.cn

[R72] 等待端口就绪
来源：http://kdu.hesvh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eib.fzhhl.top

[R73] 分割大日志
来源：http://pzp.yuanzhike.top

split -l 1000 big.log part_
来源：http://tkk.jinqigufen.top

[R74] 批量重命名
来源：http://nod.andypj.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zef.cdnleiting.top

[R75] 导出环境变量
来源：http://lqu.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://slx.fktsv.cn

[R76] 使用临时文件
来源：http://vdx.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ses.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://xfd.cheryme.top

read -rp "请输入: " ans
来源：http://tdb.xuanzx.com

[R78] 交互式菜单
来源：http://nlm.smart0.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://cxc.hfpthk.cn

[R79] 解析命令行选项
来源：http://pga.zhaomingkeji.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xuh.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://lnl.ivvv.top

time ./run.sh
来源：http://ndp.ydjk.org.cn

================================================================================
来源：http://opd.shzxlz.cn

S. C / C++ 专题
来源：http://dcc.jyoumei.cn

================================================================================
来源：http://ijv.tian-w.cn

[S01] C：Hello World
来源：http://rwf.hcnkem.com

#include <stdio.h>
来源：http://dmk.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://blz.yonumen.top

[S02] C：变量与格式化输出
来源：http://fsj.tianlin.xyz

int a = 10; printf("%d\n", a);
来源：http://vvu.gaohongyu789.top

[S03] C：读入整数
来源：http://sjh.chenlongwang.top

int x; scanf("%d", &x);
来源：http://qxd.shangyingyoupin.top

[S04] C：字符串复制
来源：http://zdy.wangshuangyany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pio.sxryk.cn

[S05] C：字符串长度
来源：http://bks.zhaomingkeji.xyz

strlen(s)
来源：http://ike.hfpthk.cn

[S06] C：字符串比较
来源：http://jwu.hcnkem.com

strcmp(a, b) == 0
来源：http://yzr.fzhhl.top

[S07] C：数组遍历求和
来源：http://zgn.ywan-chungtsiang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ptx.gaohongyu789.top

[S08] C：动态内存分配与释放
来源：http://wsq.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://scz.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://uqu.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yrv.cashguo.top

[S10] C：指针与解引用
来源：http://qum.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://dgc.redwolf501.top

[S11] C：逐行读文件
来源：http://xvb.52xcode.cn

FILE *f = fopen("a.txt", "r");
来源：http://yaf.sjlbkw.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ynd.c1oappe.top

fclose(f);
来源：http://alu.zdqjudy.top

[S12] C：写文件
来源：http://sml.ppjwa.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gug.zycfv.cn

[S13] C：宏定义
来源：http://fmf.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pht.zhoulong.xyz

[S14] C：枚举
来源：http://ess.zdqjudy.top

enum Color { RED, GREEN, BLUE };
来源：http://gpu.shzxlz.cn

[S15] C：类型转换
来源：http://shg.cheryme.top

(double) a / b
来源：http://zgd.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://jsq.zhijiandao.cn

x |= (1 << 3);
来源：http://vek.nanxuanxn.top

[S17] C：安全拼接字符串
来源：http://nms.52xcode.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sea.ivvv.top

[S18] C：命令行参数
来源：http://zgo.xylfe.cn

int main(int argc, char **argv)
来源：http://gow.aibaodan.cn

[S19] C：快速排序
来源：http://rxh.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tiz.kuanghao11.cn

[S20] C：二分查找
来源：http://nsm.daria6918.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hok.xinyue.icu

[S21] C：字符类别判断
来源：http://ink.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xya.birdmap.top

[S22] C：字符串转数字
来源：http://cvc.aizwys.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iex.sufxvd.cn

[S23] C：随机数
来源：http://aww.smart0.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://tpt.hnqzz.top

[S24] C：获取本地时间
来源：http://mya.yfazqb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yao.jinqigufen.top

[S25] C：内存拷贝
来源：http://emd.xziqi.cn

memcpy(dst, src, n);
来源：http://aho.gogol.net.cn

[S26] C：内存清零
来源：http://jwk.yueranfly.top

memset(a, 0, sizeof a);
来源：http://uhq.cqqwz.cn

[S27] C：定义常量
来源：http://vif.yueranfly.top

const double PI = 3.14159;
来源：http://lka.aizwys.cn

[S28] C：静态变量
来源：http://fgl.hywenlv.cn

static int counter = 0;
来源：http://dqk.mhx1999.top

[S29] C：变参函数
来源：http://ajv.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gjw.cashguo.top

[S30] C：头文件保护
来源：http://wfd.iojbl.cn

#ifndef X_H
来源：http://pvp.shanyushiyangtech.top

#define X_H
来源：http://icn.yj20258.top

#endif
来源：http://vxu.yanxiufei.cn

[S31] C++：Hello World
来源：http://bby.shanyushiyangkeji.top

#include <iostream>
来源：http://nfc.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://ort.yvedp.cn

[S32] C++：字符串
来源：http://tgc.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://osd.zdbjq.cn

[S33] C++：vector 增删
来源：http://dpe.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eiu.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://xxh.tarul.cn

for (auto &x : v) { std::cout << x; }
来源：http://xaz.chenjidiqi.icu

[S35] C++：map
来源：http://bxp.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kiq.hysaishi.cn

[S36] C++：unordered_map
来源：http://inp.jinqigufen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qhw.zhiwuduotai.top

[S37] C++：set
来源：http://igf.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gce.sjlbkw.cn

[S38] C++：排序
来源：http://bvt.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://tcy.cheryme.top

[S39] C++：自定义比较器排序
来源：http://fsh.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://poz.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://ium.tanke756.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tkb.jqgfzy.top

[S41] C++：类与构造函数
来源：http://gvs.bjfxy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qpc.shuidangran.top

[S42] C++：继承与虚函数
来源：http://bvd.xuanzx.com

class B : public Base { public: void f() override {} };
来源：http://zna.jiagoushi.top

[S43] C++：智能指针
来源：http://rku.jyoumei.cn

auto p = std::make_unique<int>(5);
来源：http://bws.guannengcc.top

[S44] C++：引用传参
来源：http://pop.shuidangran.top

void inc(int &x) { ++x; }
来源：http://mwq.zdqjudy.top

[S45] C++：lambda
来源：http://vue.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://gkr.meibo888.top

[S46] C++：函数模板
来源：http://wbq.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cdf.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://miq.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tif.chenzaomai.com

[S48] C++：逐行读文件
来源：http://wtm.shzxlz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://weu.yongpay.top

while (std::getline(in, line)) { }
来源：http://kge.zdbjq.cn

[S49] C++：写文件
来源：http://doq.yongpay.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vmj.zhengqikj.top

[S50] C++：格式化数字
来源：http://wpg.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xgk.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://pti.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://wvp.fengsongda.top

[S52] C++：const 与 noexcept
来源：http://yxg.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://ihx.haohaochexian.top

[S53] C++：移动语义
来源：http://pov.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://ntm.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://hij.jqgfzy.top


<!-- 参考信息 -->