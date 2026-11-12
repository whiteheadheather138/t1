代发 wailian999

[Q84] 去除首尾空格
来源：http://ldu.zhixingplan.top

SELECT TRIM(name) FROM users;
来源：http://aag.jinqigufen.top

[Q85] 数值取整
来源：http://gwa.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nvz.shanyushiyangkeji.top

[Q86] 读取 JSON 字段
来源：http://drs.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uxj.hesvh.cn

[Q87] JSON 字段做条件
来源：http://oed.ybcxt.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tsv.chenlongwang.top

[Q88] 行转列（条件聚合）
来源：http://uxs.shzxlz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qfk.xuetiantiany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aek.chenlongwang.top

[Q89] 判断表是否存在
来源：http://pfh.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://txm.cucudq.cn

[Q90] 生成序号列
来源：http://old.fktsv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wyc.xuanzx.com

================================================================================
来源：http://pnp.pengpengdd.cyou

R. Bash 专题
来源：http://oym.havefunace.top

================================================================================
来源：http://uwc.sxryk.cn

[R01] shebang 与严格模式
来源：http://plg.pycfn.com

#!/usr/bin/env bash
来源：http://ubt.hammf.cn

set -euo pipefail
来源：http://jhx.gzhubu.top

[R02] 变量赋值与使用
来源：http://sje.daria6918.cn

name="Tom"; echo "$name"
来源：http://lcz.yongpay.top

[R03] 只读变量
来源：http://drb.feifeiyinyue.top

readonly PI=3.14
来源：http://lmq.cucudq.cn

[R04] 位置参数
来源：http://mcx.xinyue.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://szt.aibaodan.cn

[R05] 参数默认值
来源：http://cyu.tanke756.top

name="${1:-default}"
来源：http://eic.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://qtr.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vjj.zhiwuduotai.top

[R07] if 判断文件
来源：http://ajs.yj202588.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tfh.uphjek.com

[R08] 数值比较
来源：http://skm.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vdu.hammf.cn

[R09] 字符串比较
来源：http://bbk.ppjwa.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xpc.ivvv.top

[R10] 正则匹配
来源：http://oky.redwolf501.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xcn.hnqzz.top

[R11] case 多分支
来源：http://qix.daria6918.cn

case "$1" in
来源：http://irb.yueranfly.top

start) echo "启动" ;;
来源：http://nfb.sxryk.cn

stop)  echo "停止" ;;
来源：http://esb.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://hpz.hnxiangtu.top

esac
来源：http://jjd.yangfankeji.com

[R12] for 遍历文件
来源：http://aes.fktsv.cn

for f in *.txt; do echo "$f"; done
来源：http://wli.aizwys.cn

[R13] for 计数循环
来源：http://rjl.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://fcq.mhx1999.top

[R14] C 风格 for
来源：http://bpr.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ijd.wangdashe.top

[R15] while 逐行读文件
来源：http://yac.andypj.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gym.dashuyun.cn

[R16] until 等待条件
来源：http://llf.zhijiandao.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kkq.snrcjt.cn

[R17] 数组定义与取值
来源：http://add.meibo888.top

arr=(a b c); echo "${arr[0]}"
来源：http://orl.jinqigfzy.top

[R18] 遍历数组
来源：http://cow.zycfv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iop.9152youxi.cn

[R19] 数组长度
来源：http://mkj.pengpengdd.cyou

echo "${#arr[@]}"
来源：http://pek.aizwys.cn

[R20] 关联数组（字典）
来源：http://ymn.shuidangran.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sds.chenjidiqi.icu

[R21] 字符串长度
来源：http://iup.jlsjyb.cn

echo "${#s}"
来源：http://mvb.nwbrower.top

[R22] 截取子串
来源：http://qmp.sweek.top

echo "${s:0:5}"
来源：http://ylc.yonumen.top

[R23] 字符串替换
来源：http://tav.wangdashe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cod.guannengcc.top

[R24] 大小写转换
来源：http://vnx.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://jgw.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://kpu.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vtm.sufxvd.cn

[R26] 命令替换
来源：http://ztr.feifeiyinyue.top

now=$(date +%F); echo "$now"
来源：http://zvg.gzhubu.top

[R27] 算术展开
来源：http://tuq.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://mmq.jianghu66.top

[R28] 浮点运算
来源：http://vlu.quarkkingdee.top

echo "scale=2; 10/3" | bc
来源：http://mkr.hongshengwenyu.top

[R29] 定义函数
来源：http://mjv.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cfs.xuanzx.com

[R30] 函数返回状态码
来源：http://wfl.ppjwa.cn

f() { return 0; }; f || echo "失败了"
来源：http://dsi.xziqi.cn

[R31] 局部变量
来源：http://hfn.zhiwuduotai.top

f() { local x=1; echo "$x"; }
来源：http://nfj.gogol.net.cn

[R32] 参数个数校验
来源：http://yrz.yangfankeji.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jtp.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://ace.9152youxi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gls.hesvh.cn

[R34] 退出时清理
来源：http://pau.zhiwuduotai.top

trap 'rm -f "$tmp"' EXIT
来源：http://cai.gotoacloud.top

[R35] 后台执行并等待
来源：http://wgr.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ddf.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://ovb.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dxg.uphjek.com

[R37] 把输出赋给变量
来源：http://xmo.sysykeji.top

files=$(ls -1)
来源：http://gvk.52xcode.cn

[R38] 管道串联
来源：http://yip.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://gsa.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://mio.tanke756.top

cmd > out.log 2>&1
来源：http://dym.cashguo.top

[R40] 追加写日志
来源：http://esa.vehdjk.com

echo "log" >> out.log
来源：http://umt.pengpengdd.cyou

[R41] 丢弃输出
来源：http://uqb.yueranfly.top

cmd >/dev/null 2>&1
来源：http://cnh.tian-w.cn

[R42] 输入重定向
来源：http://oxp.tian-w.cn

wc -l < a.txt
来源：http://uko.yuxming.cn

[R43] 按名字查找文件
来源：http://tiy.feifeiyinyue.top

find . -name "*.log" -type f
来源：http://dlf.haohaochexian.top

[R44] 按修改时间查找
来源：http://mol.chenzaomai.com

find . -mtime -7 -type f
来源：http://icj.ybcxt.top

[R45] 批量删除
来源：http://uea.bbcook.cn

find . -name "*.tmp" -delete
来源：http://vtq.ppjwa.cn

[R46] 递归替换文件内容
来源：http://fpc.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hjm.cqqwz.cn

[R47] sed 单行替换
来源：http://tjo.yueranfly.top

sed -i 's/foo/bar/g' a.txt
来源：http://qje.ppjwa.cn

[R48] awk 取指定列
来源：http://oeo.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://xhr.chenlongwang.top

[R49] awk 带条件
来源：http://nmi.gogol.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sbd.hongshengwenyu.top

[R50] awk 求和
来源：http://mmp.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gto.yvedp.cn

[R51] 排序去重取前几
来源：http://tsk.iojbl.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kxb.zhengqikj.top

[R52] 统计行数
来源：http://ysy.gogol.net.cn

wc -l a.txt
来源：http://dcn.yfazqb.com

[R53] 查看文件头与实时尾
来源：http://pws.316326.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pyr.yueranfly.top

[R54] 比较两个文件
来源：http://laf.yfazqb.com

diff a.txt b.txt
来源：http://yyu.zdqjudy.top

[R55] 压缩与解压
来源：http://xfz.gogol.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jof.yj20258888.top

[R56] 远程拷贝
来源：http://bez.hnqzz.top

scp file user@host:/path/
来源：http://sab.zhixingplan.top

[R57] 远程执行命令
来源：http://nmo.cucudq.cn

ssh user@host 'uptime'
来源：http://bkc.nanxinkj.top

[R58] 下载文件
来源：http://czh.vqdsnc.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jbo.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://gwt.ehwqpu.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://udh.ydjk.org.cn

[R60] 只看 HTTP 状态码
来源：http://ezg.zhaomingkeji.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://axw.jinghuilouyu.cn

[R61] 磁盘占用
来源：http://vvd.jqgfzy.top

df -h;  du -sh *
来源：http://ivn.sufxvd.cn

[R62] 找最占空间的文件
来源：http://yis.shuidangran.top

du -ah . | sort -rh | head -10
来源：http://xfb.yueranfly.top

[R63] 内存与进程
来源：http://jst.hesvh.cn

free -h;  ps aux | grep nginx
来源：http://ckx.xziqi.cn

[R64] 结束进程
来源：http://drn.0kj1m.cn

kill -9 $(pgrep -f app.py)
来源：http://mkb.yj20258.top

[R65] 查看端口占用
来源：http://elu.yfazqb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sro.ppjwa.cn

[R66] 定时任务
来源：http://xoy.zhaomingkeji.xyz

crontab -e;  crontab -l
来源：http://xka.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://bpv.gaohongyu789.top

openssl rand -hex 16
来源：http://hon.hnxiangtu.top

[R68] 计算文件校验值
来源：http://umu.shuidangran.top

sha256sum a.txt;  md5sum a.txt
来源：http://bcs.yuanzhike.top

[R69] 生成随机密码
来源：http://ygn.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://wgd.meibo888.top

[R70] 时间戳与互转
来源：http://rbz.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://eqo.sweek.top

[R71] 日期格式化
来源：http://col.hongshengwenyu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jyx.dianchejie.cn

[R72] 等待端口就绪
来源：http://cge.jlsjyb.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hzq.ydzc1.top

[R73] 分割大日志
来源：http://ron.cucudq.cn

split -l 1000 big.log part_
来源：http://ixg.vehdjk.com

[R74] 批量重命名
来源：http://fcg.jinyuanbaomall.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hnm.9152youxi.cn

[R75] 导出环境变量
来源：http://lpo.daria6918.cn

export PATH="$HOME/bin:$PATH"
来源：http://seb.yj20258.top

[R76] 使用临时文件
来源：http://clj.zhoulong.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rhg.chenlongwang.top

[R77] 读取用户输入
来源：http://eos.fanxiaobao.xyz

read -rp "请输入: " ans
来源：http://egz.c1oappe.top

[R78] 交互式菜单
来源：http://buj.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://zrl.sysykeji.top

[R79] 解析命令行选项
来源：http://cun.jinqigufen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ieq.yvedp.cn

[R80] 查看脚本执行耗时
来源：http://uoi.tianlin.xyz

time ./run.sh
来源：http://aic.nanxinkj.top

================================================================================
来源：http://yhd.xuetiantiany.cn

S. C / C++ 专题
来源：http://wkw.sjlbkw.cn

================================================================================
来源：http://dxe.snrcjt.cn

[S01] C：Hello World
来源：http://bji.zhaomingkeji.xyz

#include <stdio.h>
来源：http://wga.vqdsnc.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xyo.tian-w.cn

[S02] C：变量与格式化输出
来源：http://aex.shangyingyoupin.top

int a = 10; printf("%d\n", a);
来源：http://qgy.guowangkeji.top

[S03] C：读入整数
来源：http://gha.zycfv.cn

int x; scanf("%d", &x);
来源：http://ckx.sxryk.cn

[S04] C：字符串复制
来源：http://gus.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yzj.sweek.top

[S05] C：字符串长度
来源：http://kgf.shangyingyoupin.top

strlen(s)
来源：http://jcf.zhongyouzk.top

[S06] C：字符串比较
来源：http://hzj.zycfv.cn

strcmp(a, b) == 0
来源：http://csr.tarul.cn

[S07] C：数组遍历求和
来源：http://mvt.yonumen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hms.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://bst.hongshengwenyu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lrp.vehdjk.com

[S09] C：结构体定义与初始化
来源：http://zwe.ybcxt.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yjb.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://pyc.xziqi.cn

int *p = &a;  *p = 5;
来源：http://igw.sweek.top

[S11] C：逐行读文件
来源：http://jix.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://bui.shangyingyoupin.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://oyu.feifeiyinyue.top

fclose(f);
来源：http://iee.xziqi.cn

[S12] C：写文件
来源：http://rbz.yangfankeji.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dep.zdbjq.cn

[S13] C：宏定义
来源：http://hen.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tlg.jinqigfzy.top

[S14] C：枚举
来源：http://qri.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://mmo.nanxuanxn.top

[S15] C：类型转换
来源：http://zbh.xylfe.cn

(double) a / b
来源：http://yuw.gaohongyu789.top

[S16] C：位操作置位
来源：http://wtt.bbcook.cn

x |= (1 << 3);
来源：http://egw.ybcxt.top

[S17] C：安全拼接字符串
来源：http://pyb.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ybn.9152youxi.cn

[S18] C：命令行参数
来源：http://gbu.sweek.top

int main(int argc, char **argv)
来源：http://mhq.sjlbkw.cn

[S19] C：快速排序
来源：http://zaw.daxiang520.top

qsort(a, n, sizeof(int), cmp);
来源：http://lkf.yj20258.top

[S20] C：二分查找
来源：http://yfs.meibo888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uit.daxiang520.top

[S21] C：字符类别判断
来源：http://exj.sufxvd.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vmm.jlsjyb.cn

[S22] C：字符串转数字
来源：http://qpd.zhijiandao.cn

atoi("42");  strtod("3.14", NULL);
来源：http://afe.yanxiufei.cn

[S23] C：随机数
来源：http://qzb.dashuyun.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dix.sweek.top

[S24] C：获取本地时间
来源：http://ntv.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nho.ehwqpu.com

[S25] C：内存拷贝
来源：http://wcp.yongpay.top

memcpy(dst, src, n);
来源：http://cem.zhijiandao.cn

[S26] C：内存清零
来源：http://kjs.yanxiufei.cn

memset(a, 0, sizeof a);
来源：http://duu.cucudq.cn

[S27] C：定义常量
来源：http://ohv.ybcxt.top

const double PI = 3.14159;
来源：http://sfz.daxiang520.top

[S28] C：静态变量
来源：http://zdx.jlsjyb.cn

static int counter = 0;
来源：http://tvm.yongpay.top

[S29] C：变参函数
来源：http://fyu.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mni.hcnkem.com

[S30] C：头文件保护
来源：http://odk.fanxiaobao.xyz

#ifndef X_H
来源：http://kgl.gzhubu.top

#define X_H
来源：http://ack.andypj.xyz

#endif
来源：http://hmz.chenjidiqi.icu

[S31] C++：Hello World
来源：http://hzv.jqgufenzy.top

#include <iostream>
来源：http://uzk.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://twv.andypj.xyz

[S32] C++：字符串
来源：http://zdi.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://eql.xuanzx.com

[S33] C++：vector 增删
来源：http://srr.chenjidiqi.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rim.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://iqb.c1oappe.top

for (auto &x : v) { std::cout << x; }
来源：http://hhv.vqdsnc.cn

[S35] C++：map
来源：http://pny.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rpz.havefunace.top

[S36] C++：unordered_map
来源：http://ssn.uphjek.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pwd.andypj.xyz

[S37] C++：set
来源：http://xyd.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://duk.smart0.xyz

[S38] C++：排序
来源：http://snn.xinyue.icu

std::sort(v.begin(), v.end());
来源：http://fhq.epnwcf.com

[S39] C++：自定义比较器排序
来源：http://uxb.epnwcf.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nfu.gogol.net.cn

[S40] C++：查找元素
来源：http://fjk.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cte.sysykeji.top

[S41] C++：类与构造函数
来源：http://qci.nanxuanxn.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wyr.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://yqn.cqqwz.cn

class B : public Base { public: void f() override {} };
来源：http://qyl.zhijiandao.cn

[S43] C++：智能指针
来源：http://yuq.zdqjudy.top

auto p = std::make_unique<int>(5);
来源：http://aab.zycfv.cn

[S44] C++：引用传参
来源：http://jth.bjfxy.top

void inc(int &x) { ++x; }
来源：http://fkz.cqqwz.cn

[S45] C++：lambda
来源：http://dbf.yonumen.top

auto add = [](int a, int b) { return a + b; };
来源：http://gkx.tarul.cn

[S46] C++：函数模板
来源：http://glv.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wmk.pycfn.com

[S47] C++：结构化绑定遍历
来源：http://kwd.ydjk.org.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hqd.svipenyu.cn

[S48] C++：逐行读文件
来源：http://pyk.shanyushiyangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://cqc.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://noy.zhengqikj.top

[S49] C++：写文件
来源：http://zkb.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bnj.ybcxt.top

[S50] C++：格式化数字
来源：http://niy.shanyushiyangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jdp.snrcjt.cn

[S51] C++：显式类型转换
来源：http://bvc.gaohongyu789.top

static_cast<double>(a) / b
来源：http://onp.hammf.cn

[S52] C++：const 与 noexcept
来源：http://yrl.tanke756.top

int size() const noexcept { return n_; }
来源：http://rxu.epnwcf.com

[S53] C++：移动语义
来源：http://rze.tarul.cn

std::vector<int> w = std::move(v);
来源：http://saa.zhiwuduotai.top

[S54] C++：异常处理
来源：http://byk.xingfuxueyuan.xyz


<!-- 参考信息 -->