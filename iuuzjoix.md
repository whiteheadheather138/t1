代发 wailian999

[Q86] 读取 JSON 字段
来源：http://vzs.zycfv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rxe.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://gqb.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uyv.fanxiaobao.xyz

[Q88] 行转列（条件聚合）
来源：http://juc.jianghu66.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kvp.sxryk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lth.ydjk.org.cn

[Q89] 判断表是否存在
来源：http://nqg.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ehw.tarul.cn

[Q90] 生成序号列
来源：http://von.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nkh.jqgfzy.top

================================================================================
来源：http://pvf.yuanzhike.top

R. Bash 专题
来源：http://tem.shangyingyoupin.top

================================================================================
来源：http://pvc.zhijiandao.cn

[R01] shebang 与严格模式
来源：http://din.yuxming.cn

#!/usr/bin/env bash
来源：http://zez.yj20258888.top

set -euo pipefail
来源：http://qjh.zhijiandao.cn

[R02] 变量赋值与使用
来源：http://wgr.smart0.xyz

name="Tom"; echo "$name"
来源：http://oig.guannengcc.top

[R03] 只读变量
来源：http://tpj.yuanzhike.top

readonly PI=3.14
来源：http://ccp.jyoumei.cn

[R04] 位置参数
来源：http://cqi.zdbjq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pma.zhixingplan.top

[R05] 参数默认值
来源：http://twz.bbcook.cn

name="${1:-default}"
来源：http://skv.ppjwa.cn

[R06] 判断命令是否存在
来源：http://qjh.feifeiyinyue.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qnb.aibaodan.cn

[R07] if 判断文件
来源：http://iof.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qtq.sysykeji.top

[R08] 数值比较
来源：http://luj.jinyuanbaomall.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wfd.zhoulong.xyz

[R09] 字符串比较
来源：http://ggh.fengsongda.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sdg.jyoumei.cn

[R10] 正则匹配
来源：http://akl.sysykeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jas.hcnkem.com

[R11] case 多分支
来源：http://lwv.yvedp.cn

case "$1" in
来源：http://oqd.chenjidiqi.icu

start) echo "启动" ;;
来源：http://wam.bjfxy.top

stop)  echo "停止" ;;
来源：http://ksg.0kj1m.cn

*)     echo "未知命令" ;;
来源：http://ceh.zhaomingkeji.xyz

esac
来源：http://nmb.ybcxt.top

[R12] for 遍历文件
来源：http://yxw.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://irh.mhx1999.top

[R13] for 计数循环
来源：http://upy.ydjk.org.cn

for i in {1..10}; do echo "$i"; done
来源：http://rdh.sxryk.cn

[R14] C 风格 for
来源：http://mbk.gzhubu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hwo.yuxming.cn

[R15] while 逐行读文件
来源：http://urc.ctjpmb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uos.bjfxy.top

[R16] until 等待条件
来源：http://viv.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gsn.hnqzz.top

[R17] 数组定义与取值
来源：http://fii.fktsv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jdt.wangshuangyany.cn

[R18] 遍历数组
来源：http://ran.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jiu.wangshuangyany.cn

[R19] 数组长度
来源：http://txo.nanxuanxn.top

echo "${#arr[@]}"
来源：http://erf.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://htj.fehbvm.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oip.xziqi.cn

[R21] 字符串长度
来源：http://upg.andypj.xyz

echo "${#s}"
来源：http://fif.fzhhl.top

[R22] 截取子串
来源：http://hjy.hammf.cn

echo "${s:0:5}"
来源：http://jhn.hammf.cn

[R23] 字符串替换
来源：http://exb.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://acm.snrcjt.cn

[R24] 大小写转换
来源：http://crl.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://kxu.yueranfly.top

[R25] 去后缀 / 去前缀
来源：http://scl.jinqigfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uap.hywenlv.cn

[R26] 命令替换
来源：http://gvb.ybcxt.top

now=$(date +%F); echo "$now"
来源：http://ewr.yonumen.top

[R27] 算术展开
来源：http://bep.yfazqb.com

echo $((1 + 2 * 3))
来源：http://htn.cdnleiting.top

[R28] 浮点运算
来源：http://vio.fehbvm.com

echo "scale=2; 10/3" | bc
来源：http://bmf.hcnkem.com

[R29] 定义函数
来源：http://yio.aibaodan.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vsl.zhengqikj.top

[R30] 函数返回状态码
来源：http://osl.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://jqp.yanxiufei.cn

[R31] 局部变量
来源：http://hcv.mhx1999.top

f() { local x=1; echo "$x"; }
来源：http://nwd.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://gnv.mhx1999.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oto.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://gij.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bts.ppjwa.cn

[R34] 退出时清理
来源：http://gbu.cqqwz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://giu.yanxiufei.cn

[R35] 后台执行并等待
来源：http://duq.hnqzz.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pgd.tianlin.xyz

[R36] 并发执行多个任务
来源：http://zer.cqqwz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kaq.xuanzx.com

[R37] 把输出赋给变量
来源：http://fxf.snrcjt.cn

files=$(ls -1)
来源：http://cai.jiagoushi.top

[R38] 管道串联
来源：http://sxh.fanxiaobao.xyz

cat a.txt | grep -i error | wc -l
来源：http://qbk.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://ypb.vehdjk.com

cmd > out.log 2>&1
来源：http://fac.xinyue.icu

[R40] 追加写日志
来源：http://zfm.chenjidiqi.icu

echo "log" >> out.log
来源：http://fzd.gotoacloud.top

[R41] 丢弃输出
来源：http://fxx.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://hni.cashguo.top

[R42] 输入重定向
来源：http://zrr.cdnleiting.top

wc -l < a.txt
来源：http://tnf.mhx1999.top

[R43] 按名字查找文件
来源：http://oue.cucudq.cn

find . -name "*.log" -type f
来源：http://nex.sysykeji.top

[R44] 按修改时间查找
来源：http://mbl.jinqigfzy.top

find . -mtime -7 -type f
来源：http://uyn.tianlin.xyz

[R45] 批量删除
来源：http://akd.fktsv.cn

find . -name "*.tmp" -delete
来源：http://uwz.xinyue.icu

[R46] 递归替换文件内容
来源：http://ipu.hysaishi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://htr.meibo888.top

[R47] sed 单行替换
来源：http://luh.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://ubc.zhoulong.xyz

[R48] awk 取指定列
来源：http://dit.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://neo.pycfn.com

[R49] awk 带条件
来源：http://xag.snrcjt.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vtg.zdbjq.cn

[R50] awk 求和
来源：http://tjo.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uoc.zhixingplan.top

[R51] 排序去重取前几
来源：http://xzu.bbcook.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qgv.meibo888.top

[R52] 统计行数
来源：http://hsl.ydjk.org.cn

wc -l a.txt
来源：http://zqf.fanxiaobao.xyz

[R53] 查看文件头与实时尾
来源：http://ots.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hvr.52xcode.cn

[R54] 比较两个文件
来源：http://hss.cheryme.top

diff a.txt b.txt
来源：http://guu.shangyingyoupin.top

[R55] 压缩与解压
来源：http://byc.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://alv.zhengqikj.top

[R56] 远程拷贝
来源：http://hfk.hnqzz.top

scp file user@host:/path/
来源：http://pkq.cashguo.top

[R57] 远程执行命令
来源：http://rld.nwbrower.top

ssh user@host 'uptime'
来源：http://yoo.epnwcf.com

[R58] 下载文件
来源：http://lef.ydjk.org.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://krw.bjfxy.top

[R59] 发 POST JSON
来源：http://fmu.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://chn.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://gsc.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ssw.smart0.xyz

[R61] 磁盘占用
来源：http://kvx.chenlongwang.top

df -h;  du -sh *
来源：http://sls.andypj.xyz

[R62] 找最占空间的文件
来源：http://qqb.epnwcf.com

du -ah . | sort -rh | head -10
来源：http://kbz.fktsv.cn

[R63] 内存与进程
来源：http://awc.epnwcf.com

free -h;  ps aux | grep nginx
来源：http://jwk.havefunace.top

[R64] 结束进程
来源：http://ldt.tianlin.xyz

kill -9 $(pgrep -f app.py)
来源：http://kvb.zhiwuduotai.top

[R65] 查看端口占用
来源：http://hrs.quarkkingdee.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://btk.zhixingplan.top

[R66] 定时任务
来源：http://yas.fktsv.cn

crontab -e;  crontab -l
来源：http://htp.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://nfk.zhiwuduotai.top

openssl rand -hex 16
来源：http://etq.jinghuilouyu.cn

[R68] 计算文件校验值
来源：http://pva.gogol.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jni.yanxiufei.cn

[R69] 生成随机密码
来源：http://rdt.cashguo.top

head -c 16 /dev/urandom | base64
来源：http://ekt.yueranfly.top

[R70] 时间戳与互转
来源：http://qan.jinqigufen.top

date +%s;  date -d @1700000000
来源：http://onh.shanyushiyangtech.top

[R71] 日期格式化
来源：http://zfg.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bzy.jyoumei.cn

[R72] 等待端口就绪
来源：http://prw.zhoulong.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://hcu.chenlongwang.top

[R73] 分割大日志
来源：http://uey.pengpengdd.cyou

split -l 1000 big.log part_
来源：http://udi.dianchejie.cn

[R74] 批量重命名
来源：http://nce.52xcode.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dbe.hnqzz.top

[R75] 导出环境变量
来源：http://oqp.nwbrower.top

export PATH="$HOME/bin:$PATH"
来源：http://csk.bbcook.cn

[R76] 使用临时文件
来源：http://rph.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://crs.jlsjyb.cn

[R77] 读取用户输入
来源：http://ddh.fktsv.cn

read -rp "请输入: " ans
来源：http://ddj.quarkkingdee.top

[R78] 交互式菜单
来源：http://ihc.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hih.jinqigfzy.top

[R79] 解析命令行选项
来源：http://nmt.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jnw.cheryme.top

[R80] 查看脚本执行耗时
来源：http://mpo.snrcjt.cn

time ./run.sh
来源：http://gvi.haohaochexian.top

================================================================================
来源：http://dpw.jqgfzy.top

S. C / C++ 专题
来源：http://oab.zhijiandao.cn

================================================================================
来源：http://ydy.jqgufenzy.top

[S01] C：Hello World
来源：http://hfm.sweek.top

#include <stdio.h>
来源：http://nqq.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kpl.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://ohs.hcnkem.com

int a = 10; printf("%d\n", a);
来源：http://fse.xuanzx.com

[S03] C：读入整数
来源：http://dbj.yj20258.top

int x; scanf("%d", &x);
来源：http://vep.hammf.cn

[S04] C：字符串复制
来源：http://cla.epnwcf.com

char dst[32]; strcpy(dst, "hi");
来源：http://cjh.9152youxi.cn

[S05] C：字符串长度
来源：http://jmr.316326.xyz

strlen(s)
来源：http://vii.sxryk.cn

[S06] C：字符串比较
来源：http://pih.yuxming.cn

strcmp(a, b) == 0
来源：http://ysa.xinyue.icu

[S07] C：数组遍历求和
来源：http://oxi.nwbrower.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xrh.xuanzx.com

[S08] C：动态内存分配与释放
来源：http://myz.316326.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ylm.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://boq.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cax.zhaomingkeji.xyz

[S10] C：指针与解引用
来源：http://gkm.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://pxr.hammf.cn

[S11] C：逐行读文件
来源：http://toi.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://hjx.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qua.cqqwz.cn

fclose(f);
来源：http://jki.hongshengwenyu.top

[S12] C：写文件
来源：http://ugr.mhx1999.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://scc.cqqwz.cn

[S13] C：宏定义
来源：http://fkw.jinghuilouyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aef.birdmap.top

[S14] C：枚举
来源：http://hdy.316326.xyz

enum Color { RED, GREEN, BLUE };
来源：http://ykl.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://fbq.hammf.cn

(double) a / b
来源：http://xyy.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://afu.gaohongyu789.top

x |= (1 << 3);
来源：http://inx.hammf.cn

[S17] C：安全拼接字符串
来源：http://acx.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://inf.sweek.top

[S18] C：命令行参数
来源：http://bxw.snrcjt.cn

int main(int argc, char **argv)
来源：http://fbx.fanxiaobao.xyz

[S19] C：快速排序
来源：http://gkv.vehdjk.com

qsort(a, n, sizeof(int), cmp);
来源：http://gxt.chenjidiqi.icu

[S20] C：二分查找
来源：http://wmr.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hvn.tanke756.top

[S21] C：字符类别判断
来源：http://nhn.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gge.yonumen.top

[S22] C：字符串转数字
来源：http://swq.zhixingplan.top

atoi("42");  strtod("3.14", NULL);
来源：http://lzg.yvedp.cn

[S23] C：随机数
来源：http://yuc.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://bra.yvedp.cn

[S24] C：获取本地时间
来源：http://vzd.gogol.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mhk.andypj.xyz

[S25] C：内存拷贝
来源：http://adr.fzhhl.top

memcpy(dst, src, n);
来源：http://jsq.xinyue.icu

[S26] C：内存清零
来源：http://blp.zycfv.cn

memset(a, 0, sizeof a);
来源：http://uzm.zhijiandao.cn

[S27] C：定义常量
来源：http://zcw.tianlin.xyz

const double PI = 3.14159;
来源：http://sxc.chenjidiqi.icu

[S28] C：静态变量
来源：http://qfb.guowangkeji.top

static int counter = 0;
来源：http://chd.xylfe.cn

[S29] C：变参函数
来源：http://qzg.meibo888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uaa.xuetiantiany.cn

[S30] C：头文件保护
来源：http://jrd.yongpay.top

#ifndef X_H
来源：http://vjw.ydjk.org.cn

#define X_H
来源：http://yel.fehbvm.com

#endif
来源：http://xce.cheryme.top

[S31] C++：Hello World
来源：http://zxf.hammf.cn

#include <iostream>
来源：http://cmf.tian-w.cn

int main() { std::cout << "Hello\n"; }
来源：http://pru.hfpthk.cn

[S32] C++：字符串
来源：http://fjz.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://awt.dianchejie.cn

[S33] C++：vector 增删
来源：http://heq.tian-w.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://htf.ybcxt.top

[S34] C++：遍历 vector
来源：http://vpv.dianchejie.cn

for (auto &x : v) { std::cout << x; }
来源：http://frm.yonumen.top

[S35] C++：map
来源：http://dfk.quarkkingdee.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vom.bjfxy.top

[S36] C++：unordered_map
来源：http://vag.ydzc1.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bha.jqgfzy.top

[S37] C++：set
来源：http://nhi.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vqi.yuxming.cn

[S38] C++：排序
来源：http://hbp.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://dwr.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://tbe.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vxn.ehwqpu.com

[S40] C++：查找元素
来源：http://olk.tianlin.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rer.zhiwuduotai.top

[S41] C++：类与构造函数
来源：http://gmw.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rqi.ybcxt.top

[S42] C++：继承与虚函数
来源：http://qvi.hysaishi.cn

class B : public Base { public: void f() override {} };
来源：http://amo.jiagoushi.top

[S43] C++：智能指针
来源：http://chw.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://zie.hnxiangtu.top

[S44] C++：引用传参
来源：http://kve.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://bqi.havefunace.top

[S45] C++：lambda
来源：http://eee.dianchejie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bfk.ydzc1.top

[S46] C++：函数模板
来源：http://xyf.zdqjudy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nyt.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://zlb.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pry.vehdjk.com

[S48] C++：逐行读文件
来源：http://xpy.quarkkingdee.top

std::ifstream in("a.txt");  std::string line;
来源：http://tfj.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://ztw.shangyingyoupin.top

[S49] C++：写文件
来源：http://zdb.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ade.sysykeji.top

[S50] C++：格式化数字
来源：http://ipo.jinyuanbaomall.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qtw.wangdashe.top

[S51] C++：显式类型转换
来源：http://dof.cqqwz.cn

static_cast<double>(a) / b
来源：http://xla.yj20258.top

[S52] C++：const 与 noexcept
来源：http://enw.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://dmb.zhixingplan.top

[S53] C++：移动语义
来源：http://lfu.yueranfly.top

std::vector<int> w = std::move(v);
来源：http://lsb.yfazqb.com

[S54] C++：异常处理
来源：http://wzg.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pgz.yuxming.cn

[S55] C++：结构化绑定
来源：http://efe.tanke756.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kms.meibo888.top

[S56] C++：optional
来源：http://oga.birdmap.top


<!-- 参考信息 -->