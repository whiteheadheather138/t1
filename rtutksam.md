代发 wailian999

[Q86] 读取 JSON 字段
来源：http://ttp.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rip.hammf.cn

[Q87] JSON 字段做条件
来源：http://nxf.hammf.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ogu.andypj.xyz

[Q88] 行转列（条件聚合）
来源：http://xww.sysykeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ymn.aizwys.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iaz.pengpengdd.cyou

[Q89] 判断表是否存在
来源：http://ucg.epnwcf.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vbw.fzhhl.top

[Q90] 生成序号列
来源：http://psu.iojbl.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ppc.zhoulong.xyz

================================================================================
来源：http://gbd.gzhubu.top

R. Bash 专题
来源：http://fiw.ydzc1.top

================================================================================
来源：http://cok.fktsv.cn

[R01] shebang 与严格模式
来源：http://ljd.ivvv.top

#!/usr/bin/env bash
来源：http://egg.epnwcf.com

set -euo pipefail
来源：http://kpr.sysykeji.top

[R02] 变量赋值与使用
来源：http://kxm.dashuyun.cn

name="Tom"; echo "$name"
来源：http://mvj.zycfv.cn

[R03] 只读变量
来源：http://iob.jlsjyb.cn

readonly PI=3.14
来源：http://low.hcnkem.com

[R04] 位置参数
来源：http://for.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qwo.jlsjyb.cn

[R05] 参数默认值
来源：http://lty.yj20258888.top

name="${1:-default}"
来源：http://yob.nwbrower.top

[R06] 判断命令是否存在
来源：http://pyl.nanxuanxn.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kva.pengpengdd.cyou

[R07] if 判断文件
来源：http://kqc.shanyushiyangtech.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mhb.yanxiufei.cn

[R08] 数值比较
来源：http://yvg.vqdsnc.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qwe.yonumen.top

[R09] 字符串比较
来源：http://idy.yj20258888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uww.iojbl.cn

[R10] 正则匹配
来源：http://ftg.jqgufenzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lbi.iojbl.cn

[R11] case 多分支
来源：http://kgv.zdbjq.cn

case "$1" in
来源：http://sou.xuanzx.com

start) echo "启动" ;;
来源：http://obn.chenlongwang.top

stop)  echo "停止" ;;
来源：http://hap.yueranfly.top

*)     echo "未知命令" ;;
来源：http://igu.uphjek.com

esac
来源：http://tkz.chenlongwang.top

[R12] for 遍历文件
来源：http://ect.nanxuanxn.top

for f in *.txt; do echo "$f"; done
来源：http://frv.vqdsnc.cn

[R13] for 计数循环
来源：http://jyx.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://cmq.gotoacloud.top

[R14] C 风格 for
来源：http://pzr.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ncb.gogol.net.cn

[R15] while 逐行读文件
来源：http://vfn.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pzf.c1oappe.top

[R16] until 等待条件
来源：http://ozb.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mim.cdnleiting.top

[R17] 数组定义与取值
来源：http://uii.gotoacloud.top

arr=(a b c); echo "${arr[0]}"
来源：http://tpi.jqgfzy.top

[R18] 遍历数组
来源：http://jqo.xuetiantiany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://akv.redwolf501.top

[R19] 数组长度
来源：http://gtr.hcnkem.com

echo "${#arr[@]}"
来源：http://uvw.fengsongda.top

[R20] 关联数组（字典）
来源：http://zga.uphjek.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pap.zhijiandao.cn

[R21] 字符串长度
来源：http://nbl.wangdashe.top

echo "${#s}"
来源：http://ogy.xylfe.cn

[R22] 截取子串
来源：http://nhm.zycfv.cn

echo "${s:0:5}"
来源：http://zgo.shanyushiyangkeji.top

[R23] 字符串替换
来源：http://zxc.gzhubu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://orf.zhengqikj.top

[R24] 大小写转换
来源：http://tti.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://ecc.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://xjt.sweek.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vzl.pengpengdd.cyou

[R26] 命令替换
来源：http://lsg.zhaomingkeji.xyz

now=$(date +%F); echo "$now"
来源：http://lue.ehwqpu.com

[R27] 算术展开
来源：http://vtg.316326.xyz

echo $((1 + 2 * 3))
来源：http://ukl.zhiwuduotai.top

[R28] 浮点运算
来源：http://kgc.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://qiw.xinyue.icu

[R29] 定义函数
来源：http://kio.cashguo.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ggs.zhengqikj.top

[R30] 函数返回状态码
来源：http://akk.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://alf.epnwcf.com

[R31] 局部变量
来源：http://uqr.zhengqikj.top

f() { local x=1; echo "$x"; }
来源：http://lsn.yanxiufei.cn

[R32] 参数个数校验
来源：http://avq.sysykeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nri.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://vbm.jqgfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mwc.zhengqikj.top

[R34] 退出时清理
来源：http://uff.jinqigufen.top

trap 'rm -f "$tmp"' EXIT
来源：http://jpm.0kj1m.cn

[R35] 后台执行并等待
来源：http://usg.xinyue.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://jrd.zhengqikj.top

[R36] 并发执行多个任务
来源：http://ggx.nanxinkj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pjs.xuanzx.com

[R37] 把输出赋给变量
来源：http://pnr.shanyushiyangkeji.top

files=$(ls -1)
来源：http://wnv.daria6918.cn

[R38] 管道串联
来源：http://ewc.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://yws.zhoulong.xyz

[R39] 重定向标准输出与错误
来源：http://xnu.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://hqm.andypj.xyz

[R40] 追加写日志
来源：http://ezy.uphjek.com

echo "log" >> out.log
来源：http://yry.zdbjq.cn

[R41] 丢弃输出
来源：http://zym.hesvh.cn

cmd >/dev/null 2>&1
来源：http://kpq.kuanghao11.cn

[R42] 输入重定向
来源：http://tck.sysykeji.top

wc -l < a.txt
来源：http://rqe.ehwqpu.com

[R43] 按名字查找文件
来源：http://mon.zhaomingkeji.xyz

find . -name "*.log" -type f
来源：http://sdq.fengsongda.top

[R44] 按修改时间查找
来源：http://lqp.fengsongda.top

find . -mtime -7 -type f
来源：http://mcf.tianlin.xyz

[R45] 批量删除
来源：http://wkz.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://xkt.sjlbkw.cn

[R46] 递归替换文件内容
来源：http://hsm.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ifv.fehbvm.com

[R47] sed 单行替换
来源：http://tgn.daxiang520.top

sed -i 's/foo/bar/g' a.txt
来源：http://apq.hnxiangtu.top

[R48] awk 取指定列
来源：http://cgn.epnwcf.com

awk '{print $1, $3}' a.txt
来源：http://lwd.chenzaomai.com

[R49] awk 带条件
来源：http://sui.snrcjt.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qew.hnqzz.top

[R50] awk 求和
来源：http://xuu.kuanghao11.cn

awk '{s += $2} END {print s}' a.txt
来源：http://aqd.yueranfly.top

[R51] 排序去重取前几
来源：http://gpo.yuxming.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ocl.pycfn.com

[R52] 统计行数
来源：http://yqm.dashuyun.cn

wc -l a.txt
来源：http://hdg.fanxiaobao.xyz

[R53] 查看文件头与实时尾
来源：http://fvy.nanxinkj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hxc.gzhubu.top

[R54] 比较两个文件
来源：http://hhf.sjlbkw.cn

diff a.txt b.txt
来源：http://oht.xziqi.cn

[R55] 压缩与解压
来源：http://dbm.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pel.fengsongda.top

[R56] 远程拷贝
来源：http://ofu.wangdashe.top

scp file user@host:/path/
来源：http://coh.cqqwz.cn

[R57] 远程执行命令
来源：http://kdh.feifeiyinyue.top

ssh user@host 'uptime'
来源：http://gpf.0kj1m.cn

[R58] 下载文件
来源：http://uqd.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iad.zdqjudy.top

[R59] 发 POST JSON
来源：http://tul.pengpengdd.cyou

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://znl.hcnkem.com

[R60] 只看 HTTP 状态码
来源：http://aby.jyoumei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ypo.gotoacloud.top

[R61] 磁盘占用
来源：http://gjv.yongpay.top

df -h;  du -sh *
来源：http://ajm.fzhhl.top

[R62] 找最占空间的文件
来源：http://rnt.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://yey.gotoacloud.top

[R63] 内存与进程
来源：http://qwq.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://cbc.feifeiyinyue.top

[R64] 结束进程
来源：http://hap.jinqigufen.top

kill -9 $(pgrep -f app.py)
来源：http://wds.shanyushiyangkeji.top

[R65] 查看端口占用
来源：http://qkj.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://plw.quarkkingdee.top

[R66] 定时任务
来源：http://kss.birdmap.top

crontab -e;  crontab -l
来源：http://sko.yfazqb.com

[R67] 生成随机十六进制串
来源：http://mmx.sxryk.cn

openssl rand -hex 16
来源：http://mzi.gogol.net.cn

[R68] 计算文件校验值
来源：http://ylz.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://vnn.ehwqpu.com

[R69] 生成随机密码
来源：http://gqf.vqdsnc.cn

head -c 16 /dev/urandom | base64
来源：http://niv.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://emq.shangyingyoupin.top

date +%s;  date -d @1700000000
来源：http://qho.shangyingyoupin.top

[R71] 日期格式化
来源：http://yjv.uphjek.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://ufz.svipenyu.cn

[R72] 等待端口就绪
来源：http://nxs.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://aqc.ppjwa.cn

[R73] 分割大日志
来源：http://jtp.xylfe.cn

split -l 1000 big.log part_
来源：http://rzg.hcnkem.com

[R74] 批量重命名
来源：http://xxn.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rdj.ivvv.top

[R75] 导出环境变量
来源：http://vvv.vqdsnc.cn

export PATH="$HOME/bin:$PATH"
来源：http://vom.zhijiandao.cn

[R76] 使用临时文件
来源：http://afy.jlsjyb.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ksh.fktsv.cn

[R77] 读取用户输入
来源：http://jyc.chenlongwang.top

read -rp "请输入: " ans
来源：http://hay.fengsongda.top

[R78] 交互式菜单
来源：http://wch.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fph.hnqzz.top

[R79] 解析命令行选项
来源：http://vam.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qll.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://cdn.tianlin.xyz

time ./run.sh
来源：http://tqj.fengsongda.top

================================================================================
来源：http://ltk.yongpay.top

S. C / C++ 专题
来源：http://hev.haohaochexian.top

================================================================================
来源：http://vor.iojbl.cn

[S01] C：Hello World
来源：http://cwh.tanke756.top

#include <stdio.h>
来源：http://onz.sxryk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ceg.sweek.top

[S02] C：变量与格式化输出
来源：http://alv.yfazqb.com

int a = 10; printf("%d\n", a);
来源：http://ywc.ybcxt.top

[S03] C：读入整数
来源：http://enc.zdbjq.cn

int x; scanf("%d", &x);
来源：http://mww.haohaochexian.top

[S04] C：字符串复制
来源：http://drc.ydzc1.top

char dst[32]; strcpy(dst, "hi");
来源：http://nqb.jinqigfzy.top

[S05] C：字符串长度
来源：http://dws.meibo888.top

strlen(s)
来源：http://xro.hysaishi.cn

[S06] C：字符串比较
来源：http://pwx.hnqzz.top

strcmp(a, b) == 0
来源：http://zne.birdmap.top

[S07] C：数组遍历求和
来源：http://sda.daria6918.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dbd.zdbjq.cn

[S08] C：动态内存分配与释放
来源：http://sgm.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zdi.jinyuanbaomall.cn

[S09] C：结构体定义与初始化
来源：http://tqx.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nmo.pengpengdd.cyou

[S10] C：指针与解引用
来源：http://ybk.cheryme.top

int *p = &a;  *p = 5;
来源：http://brr.zhengqikj.top

[S11] C：逐行读文件
来源：http://hkz.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://cuo.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hef.fanxiaobao.xyz

fclose(f);
来源：http://usm.sufxvd.cn

[S12] C：写文件
来源：http://uzn.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://axf.andypj.xyz

[S13] C：宏定义
来源：http://cml.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xit.zhijiandao.cn

[S14] C：枚举
来源：http://vkr.guannengcc.top

enum Color { RED, GREEN, BLUE };
来源：http://cth.sweek.top

[S15] C：类型转换
来源：http://zpa.gaohongyu789.top

(double) a / b
来源：http://qmb.chenzaomai.com

[S16] C：位操作置位
来源：http://xrb.quarkkingdee.top

x |= (1 << 3);
来源：http://tzg.yueranfly.top

[S17] C：安全拼接字符串
来源：http://lpf.cqqwz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lak.yj20258.top

[S18] C：命令行参数
来源：http://ejd.xinyue.icu

int main(int argc, char **argv)
来源：http://opw.yuanzhike.top

[S19] C：快速排序
来源：http://trw.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://een.sweek.top

[S20] C：二分查找
来源：http://hje.nanxuanxn.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pac.hcnkem.com

[S21] C：字符类别判断
来源：http://qhx.pengpengdd.cyou

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qhv.chenjidiqi.icu

[S22] C：字符串转数字
来源：http://pnj.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tcc.shangyingyoupin.top

[S23] C：随机数
来源：http://ych.yangfankeji.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ohk.hnxiangtu.top

[S24] C：获取本地时间
来源：http://bvu.yj20258888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vto.hfpthk.cn

[S25] C：内存拷贝
来源：http://phk.meibo888.top

memcpy(dst, src, n);
来源：http://kha.shangyingyoupin.top

[S26] C：内存清零
来源：http://cjn.hysaishi.cn

memset(a, 0, sizeof a);
来源：http://fye.xuanzx.com

[S27] C：定义常量
来源：http://aig.wangdashe.top

const double PI = 3.14159;
来源：http://sec.dianchejie.cn

[S28] C：静态变量
来源：http://xdo.epnwcf.com

static int counter = 0;
来源：http://oud.zhaomingkeji.xyz

[S29] C：变参函数
来源：http://sbb.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yuy.tianlin.xyz

[S30] C：头文件保护
来源：http://mtk.yvedp.cn

#ifndef X_H
来源：http://oqp.andypj.xyz

#define X_H
来源：http://pzj.52xcode.cn

#endif
来源：http://jxv.zycfv.cn

[S31] C++：Hello World
来源：http://djy.daria6918.cn

#include <iostream>
来源：http://qzv.ybcxt.top

int main() { std::cout << "Hello\n"; }
来源：http://elu.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://yyv.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://pdu.shzxlz.cn

[S33] C++：vector 增删
来源：http://hxj.hcnkem.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wpg.tanke756.top

[S34] C++：遍历 vector
来源：http://zif.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://lue.tarul.cn

[S35] C++：map
来源：http://ixa.chenlongwang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uvv.ybcxt.top

[S36] C++：unordered_map
来源：http://drf.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ths.shuidangran.top

[S37] C++：set
来源：http://bus.xuetiantiany.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qfk.dianchejie.cn

[S38] C++：排序
来源：http://eja.fengsongda.top

std::sort(v.begin(), v.end());
来源：http://bdk.chenlongwang.top

[S39] C++：自定义比较器排序
来源：http://wdd.chenlongwang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qte.andypj.xyz

[S40] C++：查找元素
来源：http://equ.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uai.ppjwa.cn

[S41] C++：类与构造函数
来源：http://gxx.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://klx.jianghu66.top

[S42] C++：继承与虚函数
来源：http://hep.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://spf.yuxming.cn

[S43] C++：智能指针
来源：http://ajb.ydjk.org.cn

auto p = std::make_unique<int>(5);
来源：http://nhd.jqgfzy.top

[S44] C++：引用传参
来源：http://nkp.316326.xyz

void inc(int &x) { ++x; }
来源：http://uyf.bbcook.cn

[S45] C++：lambda
来源：http://kpm.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://yhv.snrcjt.cn

[S46] C++：函数模板
来源：http://zdv.xinyue.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kxz.shzxlz.cn

[S47] C++：结构化绑定遍历
来源：http://lmh.hammf.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uxf.mhx1999.top

[S48] C++：逐行读文件
来源：http://xqw.nwbrower.top

std::ifstream in("a.txt");  std::string line;
来源：http://tvz.ydzc1.top

while (std::getline(in, line)) { }
来源：http://rix.chenjidiqi.icu

[S49] C++：写文件
来源：http://scq.yvedp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vkg.yuanzhike.top

[S50] C++：格式化数字
来源：http://uee.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vja.epnwcf.com

[S51] C++：显式类型转换
来源：http://pyv.yanxiufei.cn

static_cast<double>(a) / b
来源：http://arc.c1oappe.top

[S52] C++：const 与 noexcept
来源：http://dpj.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://itu.hysaishi.cn

[S53] C++：移动语义
来源：http://eiu.tarul.cn

std::vector<int> w = std::move(v);
来源：http://rhe.feifeiyinyue.top

[S54] C++：异常处理
来源：http://wfj.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eqq.jyoumei.cn

[S55] C++：结构化绑定
来源：http://nkt.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://euo.yuanzhike.top

[S56] C++：optional
来源：http://xlm.tianlin.xyz


<!-- 参考信息 -->