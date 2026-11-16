代发 wailian999

[Q82] 字符长度与字节长度
来源：http://tjs.iojbl.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ajd.52xcode.cn

[Q83] 大小写转换
来源：http://mzi.hcnkem.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dmv.shuidangran.top

[Q84] 去除首尾空格
来源：http://yaj.ehwqpu.com

SELECT TRIM(name) FROM users;
来源：http://sey.snrcjt.cn

[Q85] 数值取整
来源：http://lte.jiagoushi.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lij.xziqi.cn

[Q86] 读取 JSON 字段
来源：http://ezs.chenlongwang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ogx.gotoacloud.top

[Q87] JSON 字段做条件
来源：http://lxr.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dko.hcnkem.com

[Q88] 行转列（条件聚合）
来源：http://acw.chenlongwang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ppi.jyoumei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qaf.havefunace.top

[Q89] 判断表是否存在
来源：http://idb.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lcr.zdbjq.cn

[Q90] 生成序号列
来源：http://uty.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yxo.yj20258888.top

================================================================================
来源：http://sjj.guannengcc.top

R. Bash 专题
来源：http://szf.zhiwuduotai.top

================================================================================
来源：http://zty.xziqi.cn

[R01] shebang 与严格模式
来源：http://jei.nwbrower.top

#!/usr/bin/env bash
来源：http://nfv.uphjek.com

set -euo pipefail
来源：http://fub.ydzc1.top

[R02] 变量赋值与使用
来源：http://glj.jlsjyb.cn

name="Tom"; echo "$name"
来源：http://car.shangyingyoupin.top

[R03] 只读变量
来源：http://qcr.pengpengdd.cyou

readonly PI=3.14
来源：http://djt.dashuyun.cn

[R04] 位置参数
来源：http://jme.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lio.gogol.net.cn

[R05] 参数默认值
来源：http://emk.ppjwa.cn

name="${1:-default}"
来源：http://voj.smart0.xyz

[R06] 判断命令是否存在
来源：http://whm.zhaomingkeji.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sym.jinqigfzy.top

[R07] if 判断文件
来源：http://ntx.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iuo.xziqi.cn

[R08] 数值比较
来源：http://ukv.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://qaj.cdnleiting.top

[R09] 字符串比较
来源：http://yzg.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cly.dashuyun.cn

[R10] 正则匹配
来源：http://fnv.zycfv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kui.xziqi.cn

[R11] case 多分支
来源：http://gnz.yuxming.cn

case "$1" in
来源：http://jhi.316326.xyz

start) echo "启动" ;;
来源：http://vzi.andypj.xyz

stop)  echo "停止" ;;
来源：http://kjm.xuetiantiany.cn

*)     echo "未知命令" ;;
来源：http://dax.gaohongyu789.top

esac
来源：http://hxa.cheryme.top

[R12] for 遍历文件
来源：http://hpa.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://mqw.jinqigufen.top

[R13] for 计数循环
来源：http://hzk.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://uhk.jinghuilouyu.cn

[R14] C 风格 for
来源：http://nex.zycfv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uwv.aibaodan.cn

[R15] while 逐行读文件
来源：http://lql.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wgk.cqqwz.cn

[R16] until 等待条件
来源：http://cbx.gotoacloud.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qqq.52xcode.cn

[R17] 数组定义与取值
来源：http://ski.yanxiufei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hiz.nanxinkj.top

[R18] 遍历数组
来源：http://wpk.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kww.chenlongwang.top

[R19] 数组长度
来源：http://fih.fktsv.cn

echo "${#arr[@]}"
来源：http://sze.yj20258.top

[R20] 关联数组（字典）
来源：http://wai.nanxuanxn.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gqo.hammf.cn

[R21] 字符串长度
来源：http://ltn.ydzc1.top

echo "${#s}"
来源：http://ltb.yj20258.top

[R22] 截取子串
来源：http://phw.redwolf501.top

echo "${s:0:5}"
来源：http://vhi.tianlin.xyz

[R23] 字符串替换
来源：http://qoq.guannengcc.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yws.tianlin.xyz

[R24] 大小写转换
来源：http://vou.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://sui.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://odl.wangdashe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://eqy.ybcxt.top

[R26] 命令替换
来源：http://mep.gotoacloud.top

now=$(date +%F); echo "$now"
来源：http://owk.gotoacloud.top

[R27] 算术展开
来源：http://chk.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://xng.zhaomingkeji.xyz

[R28] 浮点运算
来源：http://kcs.dashuyun.cn

echo "scale=2; 10/3" | bc
来源：http://ohz.52xcode.cn

[R29] 定义函数
来源：http://bnt.pengpengdd.cyou

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ebq.zdbjq.cn

[R30] 函数返回状态码
来源：http://hcj.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://llt.cashguo.top

[R31] 局部变量
来源：http://een.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://ltn.c1oappe.top

[R32] 参数个数校验
来源：http://aof.svipenyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dgk.shanyushiyangtech.top

[R33] 捕获错误并提示行号
来源：http://rip.sjlbkw.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xel.zdbjq.cn

[R34] 退出时清理
来源：http://ymr.cqqwz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://avs.pengpengdd.cyou

[R35] 后台执行并等待
来源：http://nlc.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://epc.bbcook.cn

[R36] 并发执行多个任务
来源：http://lxn.svipenyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pgn.guowangkeji.top

[R37] 把输出赋给变量
来源：http://red.yuxming.cn

files=$(ls -1)
来源：http://umc.feifeiyinyue.top

[R38] 管道串联
来源：http://sjc.jianghu66.top

cat a.txt | grep -i error | wc -l
来源：http://cxf.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://xfw.havefunace.top

cmd > out.log 2>&1
来源：http://fzg.sxryk.cn

[R40] 追加写日志
来源：http://wqu.vqdsnc.cn

echo "log" >> out.log
来源：http://qto.jiagoushi.top

[R41] 丢弃输出
来源：http://qzb.fktsv.cn

cmd >/dev/null 2>&1
来源：http://dgq.shuidangran.top

[R42] 输入重定向
来源：http://zoe.yuxming.cn

wc -l < a.txt
来源：http://amh.ctjpmb.com

[R43] 按名字查找文件
来源：http://rzq.xylfe.cn

find . -name "*.log" -type f
来源：http://yrc.chenjidiqi.icu

[R44] 按修改时间查找
来源：http://ghc.epnwcf.com

find . -mtime -7 -type f
来源：http://ebh.daxiang520.top

[R45] 批量删除
来源：http://rsz.sxryk.cn

find . -name "*.tmp" -delete
来源：http://dnf.jiagoushi.top

[R46] 递归替换文件内容
来源：http://tay.shanyushiyangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ncb.yonumen.top

[R47] sed 单行替换
来源：http://ovq.hesvh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://coy.nanxinkj.top

[R48] awk 取指定列
来源：http://ylt.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://pnx.zdbjq.cn

[R49] awk 带条件
来源：http://aak.zhaomingkeji.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mwf.guannengcc.top

[R50] awk 求和
来源：http://sdt.nanxinkj.top

awk '{s += $2} END {print s}' a.txt
来源：http://eil.uphjek.com

[R51] 排序去重取前几
来源：http://lbv.pengpengdd.cyou

sort a.txt | uniq -c | sort -rn | head
来源：http://wjp.yanxiufei.cn

[R52] 统计行数
来源：http://fas.havefunace.top

wc -l a.txt
来源：http://czy.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://fnd.svipenyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gpb.zhiwuduotai.top

[R54] 比较两个文件
来源：http://php.ehwqpu.com

diff a.txt b.txt
来源：http://ood.epnwcf.com

[R55] 压缩与解压
来源：http://vrn.redwolf501.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hhi.sweek.top

[R56] 远程拷贝
来源：http://zce.ehwqpu.com

scp file user@host:/path/
来源：http://klr.hcnkem.com

[R57] 远程执行命令
来源：http://tav.c1oappe.top

ssh user@host 'uptime'
来源：http://ggs.redwolf501.top

[R58] 下载文件
来源：http://ncg.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kcl.52xcode.cn

[R59] 发 POST JSON
来源：http://kjm.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gdd.yonumen.top

[R60] 只看 HTTP 状态码
来源：http://rks.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ten.0kj1m.cn

[R61] 磁盘占用
来源：http://qli.bbcook.cn

df -h;  du -sh *
来源：http://etq.yanxiufei.cn

[R62] 找最占空间的文件
来源：http://pgx.meibo888.top

du -ah . | sort -rh | head -10
来源：http://qzw.52xcode.cn

[R63] 内存与进程
来源：http://xze.zdqjudy.top

free -h;  ps aux | grep nginx
来源：http://blc.hywenlv.cn

[R64] 结束进程
来源：http://zyt.ywan-chungtsiang.top

kill -9 $(pgrep -f app.py)
来源：http://lgy.cheryme.top

[R65] 查看端口占用
来源：http://ays.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kys.gaohongyu789.top

[R66] 定时任务
来源：http://rsp.nanxinkj.top

crontab -e;  crontab -l
来源：http://bdd.hnxiangtu.top

[R67] 生成随机十六进制串
来源：http://ldi.epnwcf.com

openssl rand -hex 16
来源：http://vbq.birdmap.top

[R68] 计算文件校验值
来源：http://xgq.yj20258888.top

sha256sum a.txt;  md5sum a.txt
来源：http://kef.dashuyun.cn

[R69] 生成随机密码
来源：http://ple.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://nyn.bjfxy.top

[R70] 时间戳与互转
来源：http://hdp.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://jug.jinyuanbaomall.cn

[R71] 日期格式化
来源：http://uar.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fig.chenjidiqi.icu

[R72] 等待端口就绪
来源：http://cmm.jinqigfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rju.bjfxy.top

[R73] 分割大日志
来源：http://ahr.ydjk.org.cn

split -l 1000 big.log part_
来源：http://yak.316326.xyz

[R74] 批量重命名
来源：http://qvv.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://upe.zdqjudy.top

[R75] 导出环境变量
来源：http://ftk.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://who.haohaochexian.top

[R76] 使用临时文件
来源：http://fbw.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pnd.svipenyu.cn

[R77] 读取用户输入
来源：http://nft.cheryme.top

read -rp "请输入: " ans
来源：http://azj.zhoulong.xyz

[R78] 交互式菜单
来源：http://oai.52xcode.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fnn.chenjidiqi.icu

[R79] 解析命令行选项
来源：http://sdt.tianlin.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qji.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://bqc.jinqigufen.top

time ./run.sh
来源：http://osz.hesvh.cn

================================================================================
来源：http://fux.xingfuxueyuan.xyz

S. C / C++ 专题
来源：http://cvj.cqqwz.cn

================================================================================
来源：http://iyk.yangfankeji.com

[S01] C：Hello World
来源：http://hud.aibaodan.cn

#include <stdio.h>
来源：http://ioh.0kj1m.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ifb.shangyingyoupin.top

[S02] C：变量与格式化输出
来源：http://wfd.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://sqt.yueranfly.top

[S03] C：读入整数
来源：http://ezr.fzhhl.top

int x; scanf("%d", &x);
来源：http://ymu.52xcode.cn

[S04] C：字符串复制
来源：http://ekj.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://yjd.gaohongyu789.top

[S05] C：字符串长度
来源：http://jar.tian-w.cn

strlen(s)
来源：http://nvj.shangyingyoupin.top

[S06] C：字符串比较
来源：http://ijv.xylfe.cn

strcmp(a, b) == 0
来源：http://qud.birdmap.top

[S07] C：数组遍历求和
来源：http://ecl.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ehb.meibo888.top

[S08] C：动态内存分配与释放
来源：http://mnp.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://puf.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://fbz.cashguo.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wjf.vqdsnc.cn

[S10] C：指针与解引用
来源：http://jgc.shanyushiyangtech.top

int *p = &a;  *p = 5;
来源：http://zgl.shanyushiyangtech.top

[S11] C：逐行读文件
来源：http://thk.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://zgi.yonumen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kxn.gotoacloud.top

fclose(f);
来源：http://kpp.zhijiandao.cn

[S12] C：写文件
来源：http://owg.gaohongyu789.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://atw.sxryk.cn

[S13] C：宏定义
来源：http://uww.yuxming.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kns.kuanghao11.cn

[S14] C：枚举
来源：http://mqb.xinyue.icu

enum Color { RED, GREEN, BLUE };
来源：http://vga.havefunace.top

[S15] C：类型转换
来源：http://utj.c1oappe.top

(double) a / b
来源：http://iic.havefunace.top

[S16] C：位操作置位
来源：http://sfw.yj202588.top

x |= (1 << 3);
来源：http://vqk.shangyingyoupin.top

[S17] C：安全拼接字符串
来源：http://tnv.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vek.aibaodan.cn

[S18] C：命令行参数
来源：http://cnd.cqqwz.cn

int main(int argc, char **argv)
来源：http://rpk.uphjek.com

[S19] C：快速排序
来源：http://tdz.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://uqy.xziqi.cn

[S20] C：二分查找
来源：http://lpy.nanxuanxn.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://whf.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://olq.chenzaomai.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://udf.birdmap.top

[S22] C：字符串转数字
来源：http://wxs.zhijiandao.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dem.pycfn.com

[S23] C：随机数
来源：http://myk.gzhubu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jnq.aibaodan.cn

[S24] C：获取本地时间
来源：http://lno.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ofc.uphjek.com

[S25] C：内存拷贝
来源：http://fzy.aibaodan.cn

memcpy(dst, src, n);
来源：http://umt.jqgufenzy.top

[S26] C：内存清零
来源：http://qnv.jyoumei.cn

memset(a, 0, sizeof a);
来源：http://pdz.sysykeji.top

[S27] C：定义常量
来源：http://rhj.jinqigfzy.top

const double PI = 3.14159;
来源：http://jdv.pengpengdd.cyou

[S28] C：静态变量
来源：http://anq.sweek.top

static int counter = 0;
来源：http://dwf.snrcjt.cn

[S29] C：变参函数
来源：http://wpe.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cwy.yuanzhike.top

[S30] C：头文件保护
来源：http://kiu.cheryme.top

#ifndef X_H
来源：http://gnw.yangfankeji.com

#define X_H
来源：http://ynm.sweek.top

#endif
来源：http://bue.fehbvm.com

[S31] C++：Hello World
来源：http://wfr.sweek.top

#include <iostream>
来源：http://lve.c1oappe.top

int main() { std::cout << "Hello\n"; }
来源：http://ljs.dashuyun.cn

[S32] C++：字符串
来源：http://wof.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://jko.yanxiufei.cn

[S33] C++：vector 增删
来源：http://ibk.tianlin.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yrx.aizwys.cn

[S34] C++：遍历 vector
来源：http://ict.chenzaomai.com

for (auto &x : v) { std::cout << x; }
来源：http://sqy.cucudq.cn

[S35] C++：map
来源：http://hrz.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ium.gotoacloud.top

[S36] C++：unordered_map
来源：http://nni.yangfankeji.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ltt.shangyingyoupin.top

[S37] C++：set
来源：http://jpz.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ble.jinyuanbaomall.cn

[S38] C++：排序
来源：http://avf.yj20258.top

std::sort(v.begin(), v.end());
来源：http://hkx.tanke756.top

[S39] C++：自定义比较器排序
来源：http://pvw.yuanzhike.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nem.xylfe.cn

[S40] C++：查找元素
来源：http://car.shangyingyoupin.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cxp.daxiang520.top

[S41] C++：类与构造函数
来源：http://kyq.yj202588.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://icd.wangdashe.top

[S42] C++：继承与虚函数
来源：http://hdd.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://kps.jqgufenzy.top

[S43] C++：智能指针
来源：http://ogs.hnqzz.top

auto p = std::make_unique<int>(5);
来源：http://lom.andypj.xyz

[S44] C++：引用传参
来源：http://xql.epnwcf.com

void inc(int &x) { ++x; }
来源：http://kcr.chenlongwang.top

[S45] C++：lambda
来源：http://jdw.tarul.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lgf.52xcode.cn

[S46] C++：函数模板
来源：http://ben.xuetiantiany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eae.hnqzz.top

[S47] C++：结构化绑定遍历
来源：http://uzw.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fcg.tian-w.cn

[S48] C++：逐行读文件
来源：http://hab.uphjek.com

std::ifstream in("a.txt");  std::string line;
来源：http://nig.cashguo.top

while (std::getline(in, line)) { }
来源：http://xdf.vehdjk.com

[S49] C++：写文件
来源：http://luy.xuanzx.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qol.tian-w.cn

[S50] C++：格式化数字
来源：http://dqu.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qna.316326.xyz

[S51] C++：显式类型转换
来源：http://ubc.smart0.xyz

static_cast<double>(a) / b
来源：http://suk.shangyingyoupin.top

[S52] C++：const 与 noexcept
来源：http://wlt.gotoacloud.top


<!-- 参考信息 -->