代发 wailian999

[Q82] 字符长度与字节长度
来源：http://cff.yj202588.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fgi.andypj.xyz

[Q83] 大小写转换
来源：http://glh.fanxiaobao.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://flo.chenjidiqi.icu

[Q84] 去除首尾空格
来源：http://ios.jlsjyb.cn

SELECT TRIM(name) FROM users;
来源：http://fjk.tanke756.top

[Q85] 数值取整
来源：http://cpi.pycfn.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://llh.ybcxt.top

[Q86] 读取 JSON 字段
来源：http://hgs.sweek.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hoi.nanxuanxn.top

[Q87] JSON 字段做条件
来源：http://joz.chenjidiqi.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://udb.yanxiufei.cn

[Q88] 行转列（条件聚合）
来源：http://jbf.fzhhl.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iuh.feifeiyinyue.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zht.hammf.cn

[Q89] 判断表是否存在
来源：http://zwj.epnwcf.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sdw.epnwcf.com

[Q90] 生成序号列
来源：http://yab.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://grx.ybcxt.top

================================================================================
来源：http://glz.cqqwz.cn

R. Bash 专题
来源：http://ucb.hammf.cn

================================================================================
来源：http://lal.cdnleiting.top

[R01] shebang 与严格模式
来源：http://jnn.epnwcf.com

#!/usr/bin/env bash
来源：http://kwy.pycfn.com

set -euo pipefail
来源：http://zkt.vehdjk.com

[R02] 变量赋值与使用
来源：http://oor.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://jzg.zhengqikj.top

[R03] 只读变量
来源：http://khk.gaohongyu789.top

readonly PI=3.14
来源：http://wds.guannengcc.top

[R04] 位置参数
来源：http://jad.zhixingplan.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uht.aizwys.cn

[R05] 参数默认值
来源：http://tsq.ivvv.top

name="${1:-default}"
来源：http://olg.ppjwa.cn

[R06] 判断命令是否存在
来源：http://cha.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qjv.yanxiufei.cn

[R07] if 判断文件
来源：http://gbb.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dkx.yvedp.cn

[R08] 数值比较
来源：http://amj.jinghuilouyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wqk.chenzaomai.com

[R09] 字符串比较
来源：http://fdb.jqgfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://daa.fktsv.cn

[R10] 正则匹配
来源：http://hvo.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tvx.zhongyouzk.top

[R11] case 多分支
来源：http://bof.xziqi.cn

case "$1" in
来源：http://dux.tanke756.top

start) echo "启动" ;;
来源：http://dhf.snrcjt.cn

stop)  echo "停止" ;;
来源：http://doq.jlsjyb.cn

*)     echo "未知命令" ;;
来源：http://ngz.zhiwuduotai.top

esac
来源：http://oxo.smart0.xyz

[R12] for 遍历文件
来源：http://xwd.guowangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://ybm.cqqwz.cn

[R13] for 计数循环
来源：http://rcm.cdnleiting.top

for i in {1..10}; do echo "$i"; done
来源：http://yxo.cqqwz.cn

[R14] C 风格 for
来源：http://gsi.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zwv.fzhhl.top

[R15] while 逐行读文件
来源：http://ppx.ybcxt.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xkx.ydjk.org.cn

[R16] until 等待条件
来源：http://csq.fktsv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xtc.sxryk.cn

[R17] 数组定义与取值
来源：http://lci.ppjwa.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oat.dashuyun.cn

[R18] 遍历数组
来源：http://koz.hywenlv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qxi.xziqi.cn

[R19] 数组长度
来源：http://iqn.jianghu66.top

echo "${#arr[@]}"
来源：http://lap.yvedp.cn

[R20] 关联数组（字典）
来源：http://tfm.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pil.chenlongwang.top

[R21] 字符串长度
来源：http://pre.jianghu66.top

echo "${#s}"
来源：http://kem.fktsv.cn

[R22] 截取子串
来源：http://dpr.zycfv.cn

echo "${s:0:5}"
来源：http://rog.hnqzz.top

[R23] 字符串替换
来源：http://adb.cheryme.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rgk.jiagoushi.top

[R24] 大小写转换
来源：http://wov.nanxuanxn.top

echo "${s^^}"; echo "${s,,}"
来源：http://lpk.jqgfzy.top

[R25] 去后缀 / 去前缀
来源：http://amk.smart0.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://hxd.vehdjk.com

[R26] 命令替换
来源：http://lpk.zycfv.cn

now=$(date +%F); echo "$now"
来源：http://flr.shanyushiyangkeji.top

[R27] 算术展开
来源：http://aze.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://qhr.birdmap.top

[R28] 浮点运算
来源：http://eyr.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://gff.tanke756.top

[R29] 定义函数
来源：http://rfb.xuanzx.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://soi.fktsv.cn

[R30] 函数返回状态码
来源：http://nga.0kj1m.cn

f() { return 0; }; f || echo "失败了"
来源：http://qdi.daxiang520.top

[R31] 局部变量
来源：http://hoq.bjfxy.top

f() { local x=1; echo "$x"; }
来源：http://fqe.meibo888.top

[R32] 参数个数校验
来源：http://opj.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yse.hammf.cn

[R33] 捕获错误并提示行号
来源：http://cjd.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lax.guannengcc.top

[R34] 退出时清理
来源：http://ryg.xylfe.cn

trap 'rm -f "$tmp"' EXIT
来源：http://akx.ehwqpu.com

[R35] 后台执行并等待
来源：http://pkk.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lcc.nanxinkj.top

[R36] 并发执行多个任务
来源：http://qeo.haohaochexian.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://czh.ywan-chungtsiang.top

[R37] 把输出赋给变量
来源：http://gqe.chenjidiqi.icu

files=$(ls -1)
来源：http://gnm.zhengqikj.top

[R38] 管道串联
来源：http://shn.yj202588.top

cat a.txt | grep -i error | wc -l
来源：http://snj.yongpay.top

[R39] 重定向标准输出与错误
来源：http://nry.zhijiandao.cn

cmd > out.log 2>&1
来源：http://ngb.chenjidiqi.icu

[R40] 追加写日志
来源：http://lce.kuanghao11.cn

echo "log" >> out.log
来源：http://oiv.mhx1999.top

[R41] 丢弃输出
来源：http://owc.feifeiyinyue.top

cmd >/dev/null 2>&1
来源：http://ibv.zhijiandao.cn

[R42] 输入重定向
来源：http://xar.jinghuilouyu.cn

wc -l < a.txt
来源：http://mnp.xylfe.cn

[R43] 按名字查找文件
来源：http://gja.pycfn.com

find . -name "*.log" -type f
来源：http://flb.chenjidiqi.icu

[R44] 按修改时间查找
来源：http://iub.snrcjt.cn

find . -mtime -7 -type f
来源：http://zlk.shzxlz.cn

[R45] 批量删除
来源：http://gyz.daria6918.cn

find . -name "*.tmp" -delete
来源：http://onx.cashguo.top

[R46] 递归替换文件内容
来源：http://kym.shanyushiyangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jch.jinghuilouyu.cn

[R47] sed 单行替换
来源：http://ael.fktsv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mzi.chenlongwang.top

[R48] awk 取指定列
来源：http://xcy.fengsongda.top

awk '{print $1, $3}' a.txt
来源：http://pxi.jinqigufen.top

[R49] awk 带条件
来源：http://fib.sjlbkw.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cwh.sysykeji.top

[R50] awk 求和
来源：http://bjn.wangdashe.top

awk '{s += $2} END {print s}' a.txt
来源：http://xyd.feifeiyinyue.top

[R51] 排序去重取前几
来源：http://wgs.ydjk.org.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uax.zycfv.cn

[R52] 统计行数
来源：http://gib.316326.xyz

wc -l a.txt
来源：http://itn.yuanzhike.top

[R53] 查看文件头与实时尾
来源：http://dcs.nwbrower.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zcy.tanke756.top

[R54] 比较两个文件
来源：http://bqv.shangyingyoupin.top

diff a.txt b.txt
来源：http://oke.smart0.xyz

[R55] 压缩与解压
来源：http://cet.zhongyouzk.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nfg.gzhubu.top

[R56] 远程拷贝
来源：http://zmo.cucudq.cn

scp file user@host:/path/
来源：http://sia.epnwcf.com

[R57] 远程执行命令
来源：http://dvw.ydjk.org.cn

ssh user@host 'uptime'
来源：http://pnn.jqgufenzy.top

[R58] 下载文件
来源：http://ibx.dashuyun.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qin.xziqi.cn

[R59] 发 POST JSON
来源：http://xqa.sysykeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ahh.nwbrower.top

[R60] 只看 HTTP 状态码
来源：http://kor.aibaodan.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fvq.yonumen.top

[R61] 磁盘占用
来源：http://whk.mhx1999.top

df -h;  du -sh *
来源：http://qeq.ehwqpu.com

[R62] 找最占空间的文件
来源：http://xmc.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://khs.cqqwz.cn

[R63] 内存与进程
来源：http://ssa.meibo888.top

free -h;  ps aux | grep nginx
来源：http://mrt.ydzc1.top

[R64] 结束进程
来源：http://aha.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://bgx.smart0.xyz

[R65] 查看端口占用
来源：http://lid.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://byr.jinyuanbaomall.cn

[R66] 定时任务
来源：http://lvm.shangyingyoupin.top

crontab -e;  crontab -l
来源：http://aja.kuanghao11.cn

[R67] 生成随机十六进制串
来源：http://qim.fktsv.cn

openssl rand -hex 16
来源：http://bvb.tianlin.xyz

[R68] 计算文件校验值
来源：http://mzf.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://mny.bbcook.cn

[R69] 生成随机密码
来源：http://zji.kuanghao11.cn

head -c 16 /dev/urandom | base64
来源：http://ldr.ydjk.org.cn

[R70] 时间戳与互转
来源：http://iww.birdmap.top

date +%s;  date -d @1700000000
来源：http://zwl.zhaomingkeji.xyz

[R71] 日期格式化
来源：http://wtc.aizwys.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cli.jqgfzy.top

[R72] 等待端口就绪
来源：http://nro.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dng.hysaishi.cn

[R73] 分割大日志
来源：http://xqw.sufxvd.cn

split -l 1000 big.log part_
来源：http://nwg.aizwys.cn

[R74] 批量重命名
来源：http://kjz.316326.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zya.cucudq.cn

[R75] 导出环境变量
来源：http://xva.nanxinkj.top

export PATH="$HOME/bin:$PATH"
来源：http://kni.sufxvd.cn

[R76] 使用临时文件
来源：http://stx.shanyushiyangtech.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qin.yuanzhike.top

[R77] 读取用户输入
来源：http://ziw.shanyushiyangtech.top

read -rp "请输入: " ans
来源：http://eyr.cdnleiting.top

[R78] 交互式菜单
来源：http://mlg.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jao.316326.xyz

[R79] 解析命令行选项
来源：http://olf.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zez.wangdashe.top

[R80] 查看脚本执行耗时
来源：http://gyd.cashguo.top

time ./run.sh
来源：http://dfv.chenzaomai.com

================================================================================
来源：http://onk.ehwqpu.com

S. C / C++ 专题
来源：http://cpb.zhongyouzk.top

================================================================================
来源：http://rgr.cucudq.cn

[S01] C：Hello World
来源：http://znj.hysaishi.cn

#include <stdio.h>
来源：http://rwr.zhixingplan.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vso.zhixingplan.top

[S02] C：变量与格式化输出
来源：http://pzn.ybcxt.top

int a = 10; printf("%d\n", a);
来源：http://brg.feifeiyinyue.top

[S03] C：读入整数
来源：http://hsi.sysykeji.top

int x; scanf("%d", &x);
来源：http://bof.zycfv.cn

[S04] C：字符串复制
来源：http://npk.yuanzhike.top

char dst[32]; strcpy(dst, "hi");
来源：http://qsw.havefunace.top

[S05] C：字符串长度
来源：http://gxt.uphjek.com

strlen(s)
来源：http://nbz.xylfe.cn

[S06] C：字符串比较
来源：http://lcb.xylfe.cn

strcmp(a, b) == 0
来源：http://jun.shanyushiyangkeji.top

[S07] C：数组遍历求和
来源：http://huj.vqdsnc.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rib.aizwys.cn

[S08] C：动态内存分配与释放
来源：http://vje.yfazqb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://avq.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://oox.zhaomingkeji.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ohx.dashuyun.cn

[S10] C：指针与解引用
来源：http://afp.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://fin.fzhhl.top

[S11] C：逐行读文件
来源：http://qey.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://uhg.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yuh.zycfv.cn

fclose(f);
来源：http://edd.zhaomingkeji.xyz

[S12] C：写文件
来源：http://dpa.zhengqikj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://myb.ydzc1.top

[S13] C：宏定义
来源：http://ihf.fengsongda.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ujc.bbcook.cn

[S14] C：枚举
来源：http://cop.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://ruu.cucudq.cn

[S15] C：类型转换
来源：http://ltu.hnxiangtu.top

(double) a / b
来源：http://duq.jianghu66.top

[S16] C：位操作置位
来源：http://jei.hywenlv.cn

x |= (1 << 3);
来源：http://hhl.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://myf.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://upw.nwbrower.top

[S18] C：命令行参数
来源：http://evq.fanxiaobao.xyz

int main(int argc, char **argv)
来源：http://uxi.iojbl.cn

[S19] C：快速排序
来源：http://zmm.nanxuanxn.top

qsort(a, n, sizeof(int), cmp);
来源：http://hzb.cucudq.cn

[S20] C：二分查找
来源：http://wor.zhengqikj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zed.gzhubu.top

[S21] C：字符类别判断
来源：http://paf.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tdj.cqqwz.cn

[S22] C：字符串转数字
来源：http://fhy.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://whq.vqdsnc.cn

[S23] C：随机数
来源：http://ovq.vqdsnc.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cio.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://tta.jyoumei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sql.52xcode.cn

[S25] C：内存拷贝
来源：http://ody.sjlbkw.cn

memcpy(dst, src, n);
来源：http://gro.gogol.net.cn

[S26] C：内存清零
来源：http://yus.nwbrower.top

memset(a, 0, sizeof a);
来源：http://yqw.sxryk.cn

[S27] C：定义常量
来源：http://eri.cheryme.top

const double PI = 3.14159;
来源：http://aun.iojbl.cn

[S28] C：静态变量
来源：http://bek.bbcook.cn

static int counter = 0;
来源：http://gut.ydzc1.top

[S29] C：变参函数
来源：http://voi.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vad.fanxiaobao.xyz

[S30] C：头文件保护
来源：http://gaa.xuanzx.com

#ifndef X_H
来源：http://kel.fanxiaobao.xyz

#define X_H
来源：http://nhe.iojbl.cn

#endif
来源：http://loa.guannengcc.top

[S31] C++：Hello World
来源：http://cix.ivvv.top

#include <iostream>
来源：http://zei.yj20258.top

int main() { std::cout << "Hello\n"; }
来源：http://syd.aizwys.cn

[S32] C++：字符串
来源：http://dzm.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://tnn.ydzc1.top

[S33] C++：vector 增删
来源：http://nrs.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qxr.hywenlv.cn

[S34] C++：遍历 vector
来源：http://uln.jqgfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://zwb.zhongyouzk.top

[S35] C++：map
来源：http://rdq.gotoacloud.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nwd.dashuyun.cn

[S36] C++：unordered_map
来源：http://onn.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pkm.quarkkingdee.top

[S37] C++：set
来源：http://nru.nanxuanxn.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fit.guannengcc.top

[S38] C++：排序
来源：http://dyi.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://wbx.yj202588.top

[S39] C++：自定义比较器排序
来源：http://bre.gzhubu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wqc.birdmap.top

[S40] C++：查找元素
来源：http://cdn.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dxp.hfpthk.cn

[S41] C++：类与构造函数
来源：http://pzy.yj20258888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vwk.dashuyun.cn

[S42] C++：继承与虚函数
来源：http://lmx.316326.xyz

class B : public Base { public: void f() override {} };
来源：http://nkr.hnxiangtu.top

[S43] C++：智能指针
来源：http://nnz.sjlbkw.cn

auto p = std::make_unique<int>(5);
来源：http://uyi.sufxvd.cn

[S44] C++：引用传参
来源：http://wrz.yj202588.top

void inc(int &x) { ++x; }
来源：http://rct.aibaodan.cn

[S45] C++：lambda
来源：http://qaa.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fpc.tian-w.cn

[S46] C++：函数模板
来源：http://ecp.havefunace.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yqu.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://gfl.xinyue.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mez.ivvv.top

[S48] C++：逐行读文件
来源：http://wda.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uio.hysaishi.cn

while (std::getline(in, line)) { }
来源：http://oth.hnqzz.top

[S49] C++：写文件
来源：http://mto.tarul.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://emh.andypj.xyz

[S50] C++：格式化数字
来源：http://rvw.pengpengdd.cyou

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lvi.316326.xyz

[S51] C++：显式类型转换
来源：http://vyz.c1oappe.top

static_cast<double>(a) / b
来源：http://cgo.bjfxy.top

[S52] C++：const 与 noexcept
来源：http://eif.cqqwz.cn


<!-- 参考信息 -->