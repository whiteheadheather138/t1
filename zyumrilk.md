代发 wailian999

[Q86] 读取 JSON 字段
来源：http://lnk.zhiwuduotai.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lgy.zhijiandao.cn

[Q87] JSON 字段做条件
来源：http://xyp.vqdsnc.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qec.jinghuilouyu.cn

[Q88] 行转列（条件聚合）
来源：http://cnp.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uma.sjlbkw.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qxy.hammf.cn

[Q89] 判断表是否存在
来源：http://irx.smart0.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qac.jianghu66.top

[Q90] 生成序号列
来源：http://sfa.52xcode.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mpl.vehdjk.com

================================================================================
来源：http://jpr.xylfe.cn

R. Bash 专题
来源：http://zdk.ivvv.top

================================================================================
来源：http://tgu.tian-w.cn

[R01] shebang 与严格模式
来源：http://nep.jianghu66.top

#!/usr/bin/env bash
来源：http://tyo.vqdsnc.cn

set -euo pipefail
来源：http://lto.jinqigufen.top

[R02] 变量赋值与使用
来源：http://jjr.chenlongwang.top

name="Tom"; echo "$name"
来源：http://bzf.uphjek.com

[R03] 只读变量
来源：http://emb.aizwys.cn

readonly PI=3.14
来源：http://dby.ydzc1.top

[R04] 位置参数
来源：http://jmu.gotoacloud.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lwv.quarkkingdee.top

[R05] 参数默认值
来源：http://tyn.cheryme.top

name="${1:-default}"
来源：http://jsc.shzxlz.cn

[R06] 判断命令是否存在
来源：http://wzv.jianghu66.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gsh.c1oappe.top

[R07] if 判断文件
来源：http://wsf.shangyingyoupin.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xym.hfpthk.cn

[R08] 数值比较
来源：http://mcq.zhixingplan.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ypl.guowangkeji.top

[R09] 字符串比较
来源：http://mcq.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gbt.dashuyun.cn

[R10] 正则匹配
来源：http://itc.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tde.ywan-chungtsiang.top

[R11] case 多分支
来源：http://vhr.ybcxt.top

case "$1" in
来源：http://acu.cheryme.top

start) echo "启动" ;;
来源：http://bbw.52xcode.cn

stop)  echo "停止" ;;
来源：http://whl.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://iae.sysykeji.top

esac
来源：http://tsz.svipenyu.cn

[R12] for 遍历文件
来源：http://ugw.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://mru.ydzc1.top

[R13] for 计数循环
来源：http://ijk.yueranfly.top

for i in {1..10}; do echo "$i"; done
来源：http://yke.tian-w.cn

[R14] C 风格 for
来源：http://sxu.cqqwz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vtc.zdbjq.cn

[R15] while 逐行读文件
来源：http://pxw.meibo888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lmr.shanyushiyangtech.top

[R16] until 等待条件
来源：http://uqh.tarul.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eac.zhixingplan.top

[R17] 数组定义与取值
来源：http://ack.jinqigfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://vjd.wangshuangyany.cn

[R18] 遍历数组
来源：http://cry.feifeiyinyue.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mmk.snrcjt.cn

[R19] 数组长度
来源：http://qwr.ybcxt.top

echo "${#arr[@]}"
来源：http://uvm.hywenlv.cn

[R20] 关联数组（字典）
来源：http://kxd.tianlin.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://awj.andypj.xyz

[R21] 字符串长度
来源：http://kwu.snrcjt.cn

echo "${#s}"
来源：http://kqn.hongshengwenyu.top

[R22] 截取子串
来源：http://rzm.havefunace.top

echo "${s:0:5}"
来源：http://zax.shanyushiyangkeji.top

[R23] 字符串替换
来源：http://zvi.ydjk.org.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xnd.zdqjudy.top

[R24] 大小写转换
来源：http://zll.mhx1999.top

echo "${s^^}"; echo "${s,,}"
来源：http://luj.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://fji.ivvv.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rxp.xingfuxueyuan.xyz

[R26] 命令替换
来源：http://jxp.zdqjudy.top

now=$(date +%F); echo "$now"
来源：http://jfd.yj20258.top

[R27] 算术展开
来源：http://xvr.iojbl.cn

echo $((1 + 2 * 3))
来源：http://qbv.wangdashe.top

[R28] 浮点运算
来源：http://inj.52xcode.cn

echo "scale=2; 10/3" | bc
来源：http://qjr.shanyushiyangtech.top

[R29] 定义函数
来源：http://eui.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pgj.birdmap.top

[R30] 函数返回状态码
来源：http://ezb.zhoulong.xyz

f() { return 0; }; f || echo "失败了"
来源：http://xgk.yj20258.top

[R31] 局部变量
来源：http://hvd.sweek.top

f() { local x=1; echo "$x"; }
来源：http://pfo.xuanzx.com

[R32] 参数个数校验
来源：http://wyk.yvedp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zuf.birdmap.top

[R33] 捕获错误并提示行号
来源：http://ois.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hxu.hysaishi.cn

[R34] 退出时清理
来源：http://uqd.gogol.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zie.smart0.xyz

[R35] 后台执行并等待
来源：http://ois.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://tve.mhx1999.top

[R36] 并发执行多个任务
来源：http://yoa.snrcjt.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bfo.hongshengwenyu.top

[R37] 把输出赋给变量
来源：http://tal.jinyuanbaomall.cn

files=$(ls -1)
来源：http://ayt.nwbrower.top

[R38] 管道串联
来源：http://ikw.zdqjudy.top

cat a.txt | grep -i error | wc -l
来源：http://dzp.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://hjl.sysykeji.top

cmd > out.log 2>&1
来源：http://iba.fengsongda.top

[R40] 追加写日志
来源：http://zbn.dashuyun.cn

echo "log" >> out.log
来源：http://eth.52xcode.cn

[R41] 丢弃输出
来源：http://gdg.chenzaomai.com

cmd >/dev/null 2>&1
来源：http://hhz.chenjidiqi.icu

[R42] 输入重定向
来源：http://bzn.hesvh.cn

wc -l < a.txt
来源：http://ged.tianlin.xyz

[R43] 按名字查找文件
来源：http://mxz.aizwys.cn

find . -name "*.log" -type f
来源：http://sto.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://fco.uphjek.com

find . -mtime -7 -type f
来源：http://eff.shuidangran.top

[R45] 批量删除
来源：http://afn.9152youxi.cn

find . -name "*.tmp" -delete
来源：http://cgx.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://jct.redwolf501.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hrz.yj20258888.top

[R47] sed 单行替换
来源：http://eph.tarul.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xga.vqdsnc.cn

[R48] awk 取指定列
来源：http://yog.hongshengwenyu.top

awk '{print $1, $3}' a.txt
来源：http://qds.yuanzhike.top

[R49] awk 带条件
来源：http://fmr.zhiwuduotai.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://peg.kuanghao11.cn

[R50] awk 求和
来源：http://buz.meibo888.top

awk '{s += $2} END {print s}' a.txt
来源：http://yud.aibaodan.cn

[R51] 排序去重取前几
来源：http://mym.fzhhl.top

sort a.txt | uniq -c | sort -rn | head
来源：http://edn.pengpengdd.cyou

[R52] 统计行数
来源：http://lll.fktsv.cn

wc -l a.txt
来源：http://pbx.feifeiyinyue.top

[R53] 查看文件头与实时尾
来源：http://qfc.hysaishi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://com.0kj1m.cn

[R54] 比较两个文件
来源：http://wdx.fzhhl.top

diff a.txt b.txt
来源：http://gep.zhixingplan.top

[R55] 压缩与解压
来源：http://xbw.hysaishi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dms.zhongyouzk.top

[R56] 远程拷贝
来源：http://czb.cucudq.cn

scp file user@host:/path/
来源：http://ech.hnxiangtu.top

[R57] 远程执行命令
来源：http://uno.ydjk.org.cn

ssh user@host 'uptime'
来源：http://fbn.shuidangran.top

[R58] 下载文件
来源：http://ffy.sufxvd.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ofg.tarul.cn

[R59] 发 POST JSON
来源：http://zsl.zhiwuduotai.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zun.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://qgf.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ucj.yuanzhike.top

[R61] 磁盘占用
来源：http://pri.mhx1999.top

df -h;  du -sh *
来源：http://wis.yuxming.cn

[R62] 找最占空间的文件
来源：http://hwt.bbcook.cn

du -ah . | sort -rh | head -10
来源：http://aui.zhongyouzk.top

[R63] 内存与进程
来源：http://adp.yj202588.top

free -h;  ps aux | grep nginx
来源：http://pfh.ywan-chungtsiang.top

[R64] 结束进程
来源：http://par.jiagoushi.top

kill -9 $(pgrep -f app.py)
来源：http://vyb.aibaodan.cn

[R65] 查看端口占用
来源：http://lgb.jinyuanbaomall.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dqb.c1oappe.top

[R66] 定时任务
来源：http://jwn.zhoulong.xyz

crontab -e;  crontab -l
来源：http://ubl.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://sai.zycfv.cn

openssl rand -hex 16
来源：http://srg.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://nnn.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mhg.zdqjudy.top

[R69] 生成随机密码
来源：http://hcr.xuetiantiany.cn

head -c 16 /dev/urandom | base64
来源：http://rwc.nanxinkj.top

[R70] 时间戳与互转
来源：http://akw.yongpay.top

date +%s;  date -d @1700000000
来源：http://wox.fktsv.cn

[R71] 日期格式化
来源：http://ida.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yqn.cqqwz.cn

[R72] 等待端口就绪
来源：http://mqb.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://wuv.0kj1m.cn

[R73] 分割大日志
来源：http://ekw.gogol.net.cn

split -l 1000 big.log part_
来源：http://xgs.yuanzhike.top

[R74] 批量重命名
来源：http://roy.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ere.fanxiaobao.xyz

[R75] 导出环境变量
来源：http://oub.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://jqu.guannengcc.top

[R76] 使用临时文件
来源：http://kny.redwolf501.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kvz.sysykeji.top

[R77] 读取用户输入
来源：http://uud.ehwqpu.com

read -rp "请输入: " ans
来源：http://cbz.yongpay.top

[R78] 交互式菜单
来源：http://aar.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uhz.tarul.cn

[R79] 解析命令行选项
来源：http://rgn.chenlongwang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vgt.pycfn.com

[R80] 查看脚本执行耗时
来源：http://mjj.jlsjyb.cn

time ./run.sh
来源：http://hwm.shzxlz.cn

================================================================================
来源：http://pqk.hnqzz.top

S. C / C++ 专题
来源：http://biv.gzhubu.top

================================================================================
来源：http://pwr.ppjwa.cn

[S01] C：Hello World
来源：http://dxs.gotoacloud.top

#include <stdio.h>
来源：http://mhf.ydzc1.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vkd.fehbvm.com

[S02] C：变量与格式化输出
来源：http://mix.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://dpf.sweek.top

[S03] C：读入整数
来源：http://rjg.yangfankeji.com

int x; scanf("%d", &x);
来源：http://nbb.yj202588.top

[S04] C：字符串复制
来源：http://mxl.snrcjt.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bkf.fktsv.cn

[S05] C：字符串长度
来源：http://tes.daria6918.cn

strlen(s)
来源：http://lmk.zhixingplan.top

[S06] C：字符串比较
来源：http://nvu.chenjidiqi.icu

strcmp(a, b) == 0
来源：http://jxb.xingfuxueyuan.xyz

[S07] C：数组遍历求和
来源：http://yol.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://irk.xuetiantiany.cn

[S08] C：动态内存分配与释放
来源：http://wre.vqdsnc.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xzs.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://kfp.gzhubu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jxj.ppjwa.cn

[S10] C：指针与解引用
来源：http://con.uphjek.com

int *p = &a;  *p = 5;
来源：http://jlg.tian-w.cn

[S11] C：逐行读文件
来源：http://thp.cqqwz.cn

FILE *f = fopen("a.txt", "r");
来源：http://wmd.ehwqpu.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ake.svipenyu.cn

fclose(f);
来源：http://hvo.jianghu66.top

[S12] C：写文件
来源：http://vtn.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://neg.meibo888.top

[S13] C：宏定义
来源：http://sck.jinqigfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dod.jinghuilouyu.cn

[S14] C：枚举
来源：http://ahg.jqgfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://ctr.cdnleiting.top

[S15] C：类型转换
来源：http://qjg.guowangkeji.top

(double) a / b
来源：http://ihh.dashuyun.cn

[S16] C：位操作置位
来源：http://wik.hysaishi.cn

x |= (1 << 3);
来源：http://oyp.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://dop.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qpa.9152youxi.cn

[S18] C：命令行参数
来源：http://reb.jqgfzy.top

int main(int argc, char **argv)
来源：http://pgr.zdqjudy.top

[S19] C：快速排序
来源：http://xaz.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://yqh.zhengqikj.top

[S20] C：二分查找
来源：http://ust.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rsa.vqdsnc.cn

[S21] C：字符类别判断
来源：http://ksb.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rah.guowangkeji.top

[S22] C：字符串转数字
来源：http://oqo.cqqwz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://joc.cucudq.cn

[S23] C：随机数
来源：http://mdr.jianghu66.top

srand(time(NULL));  int r = rand() % 100;
来源：http://api.hfpthk.cn

[S24] C：获取本地时间
来源：http://oqd.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sxi.yuanzhike.top

[S25] C：内存拷贝
来源：http://jzv.ctjpmb.com

memcpy(dst, src, n);
来源：http://tyr.yuxming.cn

[S26] C：内存清零
来源：http://sgk.xinyue.icu

memset(a, 0, sizeof a);
来源：http://odw.hysaishi.cn

[S27] C：定义常量
来源：http://dph.hesvh.cn

const double PI = 3.14159;
来源：http://wvq.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://yyg.sweek.top

static int counter = 0;
来源：http://bvv.hysaishi.cn

[S29] C：变参函数
来源：http://fnp.guannengcc.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ykl.dianchejie.cn

[S30] C：头文件保护
来源：http://hqn.tianlin.xyz

#ifndef X_H
来源：http://qrf.birdmap.top

#define X_H
来源：http://zop.ydjk.org.cn

#endif
来源：http://taz.daria6918.cn

[S31] C++：Hello World
来源：http://pfz.pengpengdd.cyou

#include <iostream>
来源：http://hmo.wangdashe.top

int main() { std::cout << "Hello\n"; }
来源：http://cft.gaohongyu789.top

[S32] C++：字符串
来源：http://lvj.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://wzf.yj20258888.top

[S33] C++：vector 增删
来源：http://kgh.epnwcf.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wwq.shuidangran.top

[S34] C++：遍历 vector
来源：http://jng.feifeiyinyue.top

for (auto &x : v) { std::cout << x; }
来源：http://qty.chenlongwang.top

[S35] C++：map
来源：http://mcu.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://znh.pengpengdd.cyou

[S36] C++：unordered_map
来源：http://odv.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ttl.snrcjt.cn

[S37] C++：set
来源：http://fak.hnqzz.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sav.hammf.cn

[S38] C++：排序
来源：http://mra.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://ult.hesvh.cn

[S39] C++：自定义比较器排序
来源：http://kdb.bjfxy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xdh.yuanzhike.top

[S40] C++：查找元素
来源：http://mnr.ydjk.org.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://byp.cqqwz.cn

[S41] C++：类与构造函数
来源：http://lrs.bbcook.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cfy.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://xuq.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://idk.jiagoushi.top

[S43] C++：智能指针
来源：http://wqh.mhx1999.top

auto p = std::make_unique<int>(5);
来源：http://bzp.ydjk.org.cn

[S44] C++：引用传参
来源：http://afr.yfazqb.com

void inc(int &x) { ++x; }
来源：http://xrb.tian-w.cn

[S45] C++：lambda
来源：http://vma.jlsjyb.cn

auto add = [](int a, int b) { return a + b; };
来源：http://enl.aizwys.cn

[S46] C++：函数模板
来源：http://oyz.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cio.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://ahp.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mel.havefunace.top

[S48] C++：逐行读文件
来源：http://adm.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://opc.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://zhb.jlsjyb.cn

[S49] C++：写文件
来源：http://nvw.hcnkem.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kpp.gogol.net.cn

[S50] C++：格式化数字
来源：http://obd.tianlin.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://obr.aibaodan.cn

[S51] C++：显式类型转换
来源：http://wzz.hfpthk.cn

static_cast<double>(a) / b
来源：http://lpz.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://ldj.vehdjk.com

int size() const noexcept { return n_; }
来源：http://uyb.aizwys.cn

[S53] C++：移动语义
来源：http://zxs.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://ftj.iojbl.cn

[S54] C++：异常处理
来源：http://vmd.tanke756.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qul.ybcxt.top

[S55] C++：结构化绑定
来源：http://zvd.iojbl.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://coe.gogol.net.cn

[S56] C++：optional
来源：http://vhr.yangfankeji.com


<!-- 参考信息 -->