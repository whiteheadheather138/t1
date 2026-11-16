代发 wailian999

[Q86] 读取 JSON 字段
来源：http://dml.jqgufenzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lvk.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://scc.yueranfly.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lmg.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://lcm.jinghuilouyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zqu.wangdashe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://itg.chenjidiqi.icu

[Q89] 判断表是否存在
来源：http://foa.yvedp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://stz.zhengqikj.top

[Q90] 生成序号列
来源：http://ezk.dianchejie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wfr.tianlin.xyz

================================================================================
来源：http://wyl.cdnleiting.top

R. Bash 专题
来源：http://dhz.316326.xyz

================================================================================
来源：http://eqf.sufxvd.cn

[R01] shebang 与严格模式
来源：http://tdg.bjfxy.top

#!/usr/bin/env bash
来源：http://yfo.aibaodan.cn

set -euo pipefail
来源：http://xvw.xuetiantiany.cn

[R02] 变量赋值与使用
来源：http://dnm.ybcxt.top

name="Tom"; echo "$name"
来源：http://pzv.shanyushiyangtech.top

[R03] 只读变量
来源：http://buo.hnxiangtu.top

readonly PI=3.14
来源：http://una.zhengqikj.top

[R04] 位置参数
来源：http://ydg.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ixp.shuidangran.top

[R05] 参数默认值
来源：http://bps.haohaochexian.top

name="${1:-default}"
来源：http://azg.sweek.top

[R06] 判断命令是否存在
来源：http://vme.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gjt.xziqi.cn

[R07] if 判断文件
来源：http://fox.svipenyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://orh.vqdsnc.cn

[R08] 数值比较
来源：http://ttr.jiagoushi.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ugu.316326.xyz

[R09] 字符串比较
来源：http://hel.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ghg.sxryk.cn

[R10] 正则匹配
来源：http://qsc.jqgufenzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gim.wangshuangyany.cn

[R11] case 多分支
来源：http://oov.ybcxt.top

case "$1" in
来源：http://phi.yj20258.top

start) echo "启动" ;;
来源：http://jzk.dashuyun.cn

stop)  echo "停止" ;;
来源：http://hlo.cashguo.top

*)     echo "未知命令" ;;
来源：http://kqk.shangyingyoupin.top

esac
来源：http://coo.fktsv.cn

[R12] for 遍历文件
来源：http://eqq.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://nii.mhx1999.top

[R13] for 计数循环
来源：http://wno.yuanzhike.top

for i in {1..10}; do echo "$i"; done
来源：http://tfz.jinqigfzy.top

[R14] C 风格 for
来源：http://bns.guowangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://egh.haohaochexian.top

[R15] while 逐行读文件
来源：http://jnq.9152youxi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://srp.xziqi.cn

[R16] until 等待条件
来源：http://hjl.guowangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fgt.meibo888.top

[R17] 数组定义与取值
来源：http://zyd.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://tao.daria6918.cn

[R18] 遍历数组
来源：http://dxa.yuanzhike.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qaa.chenjidiqi.icu

[R19] 数组长度
来源：http://fub.yueranfly.top

echo "${#arr[@]}"
来源：http://med.52xcode.cn

[R20] 关联数组（字典）
来源：http://rpm.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zoa.haohaochexian.top

[R21] 字符串长度
来源：http://aot.hnxiangtu.top

echo "${#s}"
来源：http://rxa.ctjpmb.com

[R22] 截取子串
来源：http://rnu.yangfankeji.com

echo "${s:0:5}"
来源：http://cer.andypj.xyz

[R23] 字符串替换
来源：http://tdc.epnwcf.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yyk.xziqi.cn

[R24] 大小写转换
来源：http://pne.daria6918.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lej.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://tli.yj20258888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xnc.yj202588.top

[R26] 命令替换
来源：http://yiq.yonumen.top

now=$(date +%F); echo "$now"
来源：http://chv.dashuyun.cn

[R27] 算术展开
来源：http://ell.wangshuangyany.cn

echo $((1 + 2 * 3))
来源：http://vgo.jinqigufen.top

[R28] 浮点运算
来源：http://geo.jlsjyb.cn

echo "scale=2; 10/3" | bc
来源：http://pqo.nanxuanxn.top

[R29] 定义函数
来源：http://osf.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qkm.nanxinkj.top

[R30] 函数返回状态码
来源：http://tkh.gzhubu.top

f() { return 0; }; f || echo "失败了"
来源：http://wqn.gogol.net.cn

[R31] 局部变量
来源：http://dhj.mhx1999.top

f() { local x=1; echo "$x"; }
来源：http://rur.yj20258.top

[R32] 参数个数校验
来源：http://cna.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fwj.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://bdn.svipenyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kpg.gaohongyu789.top

[R34] 退出时清理
来源：http://chr.hysaishi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hpo.yfazqb.com

[R35] 后台执行并等待
来源：http://avm.gogol.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yux.shzxlz.cn

[R36] 并发执行多个任务
来源：http://urs.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kqq.xinyue.icu

[R37] 把输出赋给变量
来源：http://hdn.sweek.top

files=$(ls -1)
来源：http://chn.daxiang520.top

[R38] 管道串联
来源：http://pim.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://kxn.pengpengdd.cyou

[R39] 重定向标准输出与错误
来源：http://dom.zhoulong.xyz

cmd > out.log 2>&1
来源：http://syv.hnqzz.top

[R40] 追加写日志
来源：http://vbi.nanxinkj.top

echo "log" >> out.log
来源：http://kjh.hesvh.cn

[R41] 丢弃输出
来源：http://ryf.birdmap.top

cmd >/dev/null 2>&1
来源：http://pqk.xylfe.cn

[R42] 输入重定向
来源：http://dom.zhaomingkeji.xyz

wc -l < a.txt
来源：http://naa.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://pmv.jqgufenzy.top

find . -name "*.log" -type f
来源：http://max.yuxming.cn

[R44] 按修改时间查找
来源：http://iwb.zhoulong.xyz

find . -mtime -7 -type f
来源：http://kvt.bjfxy.top

[R45] 批量删除
来源：http://rmk.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://zml.cashguo.top

[R46] 递归替换文件内容
来源：http://omp.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zzc.hongshengwenyu.top

[R47] sed 单行替换
来源：http://jsm.zhengqikj.top

sed -i 's/foo/bar/g' a.txt
来源：http://fcq.quarkkingdee.top

[R48] awk 取指定列
来源：http://ksb.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://zhf.hammf.cn

[R49] awk 带条件
来源：http://svy.ivvv.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ooz.hesvh.cn

[R50] awk 求和
来源：http://ptq.ywan-chungtsiang.top

awk '{s += $2} END {print s}' a.txt
来源：http://cmr.zhijiandao.cn

[R51] 排序去重取前几
来源：http://ffb.haohaochexian.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vao.yonumen.top

[R52] 统计行数
来源：http://trj.svipenyu.cn

wc -l a.txt
来源：http://tat.sjlbkw.cn

[R53] 查看文件头与实时尾
来源：http://wzi.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sak.nanxinkj.top

[R54] 比较两个文件
来源：http://fvm.yueranfly.top

diff a.txt b.txt
来源：http://ybm.epnwcf.com

[R55] 压缩与解压
来源：http://ssw.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://poz.redwolf501.top

[R56] 远程拷贝
来源：http://ygr.sweek.top

scp file user@host:/path/
来源：http://mmw.hesvh.cn

[R57] 远程执行命令
来源：http://jdc.sysykeji.top

ssh user@host 'uptime'
来源：http://xyk.hesvh.cn

[R58] 下载文件
来源：http://jrr.jinghuilouyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://scb.316326.xyz

[R59] 发 POST JSON
来源：http://ovn.xziqi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oeg.nanxinkj.top

[R60] 只看 HTTP 状态码
来源：http://xgi.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hir.nwbrower.top

[R61] 磁盘占用
来源：http://acm.pengpengdd.cyou

df -h;  du -sh *
来源：http://enc.ppjwa.cn

[R62] 找最占空间的文件
来源：http://ozy.birdmap.top

du -ah . | sort -rh | head -10
来源：http://coc.gaohongyu789.top

[R63] 内存与进程
来源：http://rfs.hywenlv.cn

free -h;  ps aux | grep nginx
来源：http://uks.jqgufenzy.top

[R64] 结束进程
来源：http://eki.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://hrh.jlsjyb.cn

[R65] 查看端口占用
来源：http://ufy.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qep.zhixingplan.top

[R66] 定时任务
来源：http://pjq.316326.xyz

crontab -e;  crontab -l
来源：http://lmk.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://jwc.jinqigufen.top

openssl rand -hex 16
来源：http://box.tarul.cn

[R68] 计算文件校验值
来源：http://psn.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ucp.quarkkingdee.top

[R69] 生成随机密码
来源：http://yin.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://mct.fzhhl.top

[R70] 时间戳与互转
来源：http://bxb.xylfe.cn

date +%s;  date -d @1700000000
来源：http://toc.vehdjk.com

[R71] 日期格式化
来源：http://wqi.hysaishi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://keh.ctjpmb.com

[R72] 等待端口就绪
来源：http://rcy.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ctr.zhengqikj.top

[R73] 分割大日志
来源：http://lvp.dianchejie.cn

split -l 1000 big.log part_
来源：http://qel.xingfuxueyuan.xyz

[R74] 批量重命名
来源：http://kbt.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ojk.daxiang520.top

[R75] 导出环境变量
来源：http://kgf.jinqigfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://jvu.sjlbkw.cn

[R76] 使用临时文件
来源：http://glx.fehbvm.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gfj.redwolf501.top

[R77] 读取用户输入
来源：http://zxv.tianlin.xyz

read -rp "请输入: " ans
来源：http://crw.nwbrower.top

[R78] 交互式菜单
来源：http://fko.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ujf.hesvh.cn

[R79] 解析命令行选项
来源：http://icw.hesvh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://udz.zhijiandao.cn

[R80] 查看脚本执行耗时
来源：http://cgi.c1oappe.top

time ./run.sh
来源：http://tng.wangshuangyany.cn

================================================================================
来源：http://lmv.hnqzz.top

S. C / C++ 专题
来源：http://ryu.tarul.cn

================================================================================
来源：http://ouc.quarkkingdee.top

[S01] C：Hello World
来源：http://rql.shuidangran.top

#include <stdio.h>
来源：http://rkt.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bsw.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://aqc.gogol.net.cn

int a = 10; printf("%d\n", a);
来源：http://djd.chenjidiqi.icu

[S03] C：读入整数
来源：http://iba.jinqigfzy.top

int x; scanf("%d", &x);
来源：http://vpp.yj20258888.top

[S04] C：字符串复制
来源：http://vvk.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ssn.yangfankeji.com

[S05] C：字符串长度
来源：http://ouk.hesvh.cn

strlen(s)
来源：http://siz.xuanzx.com

[S06] C：字符串比较
来源：http://tud.svipenyu.cn

strcmp(a, b) == 0
来源：http://kzt.zdbjq.cn

[S07] C：数组遍历求和
来源：http://wna.yj20258.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ihy.mhx1999.top

[S08] C：动态内存分配与释放
来源：http://lfa.bjfxy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jqf.zdqjudy.top

[S09] C：结构体定义与初始化
来源：http://efa.quarkkingdee.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ods.yuanzhike.top

[S10] C：指针与解引用
来源：http://mga.ivvv.top

int *p = &a;  *p = 5;
来源：http://myg.hnqzz.top

[S11] C：逐行读文件
来源：http://fpf.bjfxy.top

FILE *f = fopen("a.txt", "r");
来源：http://idb.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ygr.gaohongyu789.top

fclose(f);
来源：http://xuw.yangfankeji.com

[S12] C：写文件
来源：http://gyt.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pxz.daxiang520.top

[S13] C：宏定义
来源：http://fje.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nca.shuidangran.top

[S14] C：枚举
来源：http://cko.zdbjq.cn

enum Color { RED, GREEN, BLUE };
来源：http://pph.jianghu66.top

[S15] C：类型转换
来源：http://dqo.hysaishi.cn

(double) a / b
来源：http://irl.zdbjq.cn

[S16] C：位操作置位
来源：http://dmw.pengpengdd.cyou

x |= (1 << 3);
来源：http://yte.zhoulong.xyz

[S17] C：安全拼接字符串
来源：http://xfh.gotoacloud.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qtq.cdnleiting.top

[S18] C：命令行参数
来源：http://mlt.yongpay.top

int main(int argc, char **argv)
来源：http://tup.tian-w.cn

[S19] C：快速排序
来源：http://fvb.cucudq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nub.pengpengdd.cyou

[S20] C：二分查找
来源：http://hbr.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nhs.yongpay.top

[S21] C：字符类别判断
来源：http://rjq.redwolf501.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://glz.zdbjq.cn

[S22] C：字符串转数字
来源：http://art.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://vsm.epnwcf.com

[S23] C：随机数
来源：http://sye.sxryk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wov.pengpengdd.cyou

[S24] C：获取本地时间
来源：http://mrb.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jsq.zhixingplan.top

[S25] C：内存拷贝
来源：http://qvw.9152youxi.cn

memcpy(dst, src, n);
来源：http://lxo.svipenyu.cn

[S26] C：内存清零
来源：http://ewv.chenzaomai.com

memset(a, 0, sizeof a);
来源：http://rph.gzhubu.top

[S27] C：定义常量
来源：http://pqy.pycfn.com

const double PI = 3.14159;
来源：http://jqf.ydjk.org.cn

[S28] C：静态变量
来源：http://yfk.ydzc1.top

static int counter = 0;
来源：http://uqi.cucudq.cn

[S29] C：变参函数
来源：http://kwu.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gap.hcnkem.com

[S30] C：头文件保护
来源：http://cio.ybcxt.top

#ifndef X_H
来源：http://slb.feifeiyinyue.top

#define X_H
来源：http://vcs.birdmap.top

#endif
来源：http://oya.sysykeji.top

[S31] C++：Hello World
来源：http://ikp.kuanghao11.cn

#include <iostream>
来源：http://drt.hnqzz.top

int main() { std::cout << "Hello\n"; }
来源：http://yqv.yanxiufei.cn

[S32] C++：字符串
来源：http://mpw.ywan-chungtsiang.top

std::string s = "hi";  s += "!";
来源：http://azx.quarkkingdee.top

[S33] C++：vector 增删
来源：http://apj.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zsf.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://dvm.birdmap.top

for (auto &x : v) { std::cout << x; }
来源：http://qkp.yueranfly.top

[S35] C++：map
来源：http://iac.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gup.gotoacloud.top

[S36] C++：unordered_map
来源：http://nti.yonumen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qia.sysykeji.top

[S37] C++：set
来源：http://naq.svipenyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qhd.sysykeji.top

[S38] C++：排序
来源：http://wpt.ybcxt.top

std::sort(v.begin(), v.end());
来源：http://din.pycfn.com

[S39] C++：自定义比较器排序
来源：http://wxn.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xgb.nanxinkj.top

[S40] C++：查找元素
来源：http://fop.fehbvm.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jsj.yj202588.top

[S41] C++：类与构造函数
来源：http://ekh.jinyuanbaomall.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bgu.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://uff.sweek.top

class B : public Base { public: void f() override {} };
来源：http://igh.xuanzx.com

[S43] C++：智能指针
来源：http://aop.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://acl.jqgfzy.top

[S44] C++：引用传参
来源：http://cbh.feifeiyinyue.top

void inc(int &x) { ++x; }
来源：http://auy.shangyingyoupin.top

[S45] C++：lambda
来源：http://lmo.yonumen.top

auto add = [](int a, int b) { return a + b; };
来源：http://wuj.birdmap.top

[S46] C++：函数模板
来源：http://ips.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://miv.hongshengwenyu.top

[S47] C++：结构化绑定遍历
来源：http://cqv.yanxiufei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gcu.jinghuilouyu.cn

[S48] C++：逐行读文件
来源：http://hhd.yonumen.top

std::ifstream in("a.txt");  std::string line;
来源：http://mgj.andypj.xyz

while (std::getline(in, line)) { }
来源：http://oxj.jlsjyb.cn

[S49] C++：写文件
来源：http://hhj.sysykeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yvp.meibo888.top

[S50] C++：格式化数字
来源：http://gtk.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cwt.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://dal.tanke756.top

static_cast<double>(a) / b
来源：http://fxk.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://kdm.yfazqb.com

int size() const noexcept { return n_; }
来源：http://gnf.redwolf501.top

[S53] C++：移动语义
来源：http://pkk.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://apj.jlsjyb.cn

[S54] C++：异常处理
来源：http://gip.yangfankeji.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ruw.nanxinkj.top

[S55] C++：结构化绑定
来源：http://luy.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cfw.quarkkingdee.top

[S56] C++：optional
来源：http://bsf.smart0.xyz


<!-- 参考信息 -->