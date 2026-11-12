代发 wailian999

[Q82] 字符长度与字节长度
来源：http://poq.quarkkingdee.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dru.daria6918.cn

[Q83] 大小写转换
来源：http://far.cucudq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zoc.ydzc1.top

[Q84] 去除首尾空格
来源：http://hmn.redwolf501.top

SELECT TRIM(name) FROM users;
来源：http://tcu.cdnleiting.top

[Q85] 数值取整
来源：http://bui.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wig.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://hjl.vehdjk.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wjb.jinqigfzy.top

[Q87] JSON 字段做条件
来源：http://tmc.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xgi.cheryme.top

[Q88] 行转列（条件聚合）
来源：http://oxr.ivvv.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://arl.shangyingyoupin.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rqm.shuidangran.top

[Q89] 判断表是否存在
来源：http://edh.yj20258.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ioc.daxiang520.top

[Q90] 生成序号列
来源：http://ijk.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qjh.ppjwa.cn

================================================================================
来源：http://hgq.nwbrower.top

R. Bash 专题
来源：http://iuu.birdmap.top

================================================================================
来源：http://eup.jinqigufen.top

[R01] shebang 与严格模式
来源：http://caw.316326.xyz

#!/usr/bin/env bash
来源：http://qqt.xuetiantiany.cn

set -euo pipefail
来源：http://ipe.mhx1999.top

[R02] 变量赋值与使用
来源：http://loh.yvedp.cn

name="Tom"; echo "$name"
来源：http://cpz.jinqigufen.top

[R03] 只读变量
来源：http://rkc.sxryk.cn

readonly PI=3.14
来源：http://bws.chenzaomai.com

[R04] 位置参数
来源：http://mov.sysykeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ymo.tianlin.xyz

[R05] 参数默认值
来源：http://agh.sysykeji.top

name="${1:-default}"
来源：http://deg.zycfv.cn

[R06] 判断命令是否存在
来源：http://xxy.hnqzz.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tvb.jyoumei.cn

[R07] if 判断文件
来源：http://epc.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hal.xinyue.icu

[R08] 数值比较
来源：http://vyr.ehwqpu.com

if (( a > b )); then echo "a 更大"; fi
来源：http://jnf.zhijiandao.cn

[R09] 字符串比较
来源：http://was.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://egw.tarul.cn

[R10] 正则匹配
来源：http://vex.jiagoushi.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yrr.jinghuilouyu.cn

[R11] case 多分支
来源：http://gqv.ydzc1.top

case "$1" in
来源：http://ozq.xingfuxueyuan.xyz

start) echo "启动" ;;
来源：http://hoc.guowangkeji.top

stop)  echo "停止" ;;
来源：http://mia.zhixingplan.top

*)     echo "未知命令" ;;
来源：http://mmn.yangfankeji.com

esac
来源：http://upa.gaohongyu789.top

[R12] for 遍历文件
来源：http://ilz.pycfn.com

for f in *.txt; do echo "$f"; done
来源：http://hii.hesvh.cn

[R13] for 计数循环
来源：http://qjj.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://xbo.ybcxt.top

[R14] C 风格 for
来源：http://cph.birdmap.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wxw.svipenyu.cn

[R15] while 逐行读文件
来源：http://zmk.nanxinkj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://euy.ydzc1.top

[R16] until 等待条件
来源：http://nbr.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zrv.jqgfzy.top

[R17] 数组定义与取值
来源：http://ozp.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://lwp.zdqjudy.top

[R18] 遍历数组
来源：http://mhh.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nyr.cdnleiting.top

[R19] 数组长度
来源：http://tva.smart0.xyz

echo "${#arr[@]}"
来源：http://trh.aibaodan.cn

[R20] 关联数组（字典）
来源：http://ttd.chenzaomai.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yrl.vehdjk.com

[R21] 字符串长度
来源：http://pzs.daxiang520.top

echo "${#s}"
来源：http://pql.gzhubu.top

[R22] 截取子串
来源：http://hfw.hcnkem.com

echo "${s:0:5}"
来源：http://lhh.ydzc1.top

[R23] 字符串替换
来源：http://tnt.gzhubu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iba.xuanzx.com

[R24] 大小写转换
来源：http://omv.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://jio.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://unf.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gdg.yongpay.top

[R26] 命令替换
来源：http://ony.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://mvh.sweek.top

[R27] 算术展开
来源：http://gbo.yangfankeji.com

echo $((1 + 2 * 3))
来源：http://aak.hysaishi.cn

[R28] 浮点运算
来源：http://kmg.shuidangran.top

echo "scale=2; 10/3" | bc
来源：http://vxj.zhongyouzk.top

[R29] 定义函数
来源：http://ebb.yongpay.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zzj.fktsv.cn

[R30] 函数返回状态码
来源：http://kof.cheryme.top

f() { return 0; }; f || echo "失败了"
来源：http://qst.smart0.xyz

[R31] 局部变量
来源：http://aay.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://nmz.shzxlz.cn

[R32] 参数个数校验
来源：http://ghc.xuanzx.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ftg.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://yon.jinyuanbaomall.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cwl.xylfe.cn

[R34] 退出时清理
来源：http://iir.hfpthk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fcr.tanke756.top

[R35] 后台执行并等待
来源：http://ujr.tarul.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://irx.shuidangran.top

[R36] 并发执行多个任务
来源：http://jlx.tian-w.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ikk.zhaomingkeji.xyz

[R37] 把输出赋给变量
来源：http://xkm.jinghuilouyu.cn

files=$(ls -1)
来源：http://xhe.birdmap.top

[R38] 管道串联
来源：http://jug.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://ygo.epnwcf.com

[R39] 重定向标准输出与错误
来源：http://fkk.jlsjyb.cn

cmd > out.log 2>&1
来源：http://oyk.feifeiyinyue.top

[R40] 追加写日志
来源：http://dpq.xinyue.icu

echo "log" >> out.log
来源：http://gwi.zdbjq.cn

[R41] 丢弃输出
来源：http://enr.jqgfzy.top

cmd >/dev/null 2>&1
来源：http://obz.shzxlz.cn

[R42] 输入重定向
来源：http://yiu.sufxvd.cn

wc -l < a.txt
来源：http://qlr.hywenlv.cn

[R43] 按名字查找文件
来源：http://gbe.ydjk.org.cn

find . -name "*.log" -type f
来源：http://bwg.zhijiandao.cn

[R44] 按修改时间查找
来源：http://qvc.yj202588.top

find . -mtime -7 -type f
来源：http://lia.yongpay.top

[R45] 批量删除
来源：http://jkx.cashguo.top

find . -name "*.tmp" -delete
来源：http://ojt.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://cdr.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://svl.zhongyouzk.top

[R47] sed 单行替换
来源：http://mnk.aizwys.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fze.yanxiufei.cn

[R48] awk 取指定列
来源：http://oej.gaohongyu789.top

awk '{print $1, $3}' a.txt
来源：http://fsu.smart0.xyz

[R49] awk 带条件
来源：http://aww.bjfxy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fls.yuxming.cn

[R50] awk 求和
来源：http://piw.sxryk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://twi.yonumen.top

[R51] 排序去重取前几
来源：http://ekm.cheryme.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cvy.yj20258888.top

[R52] 统计行数
来源：http://zlv.tarul.cn

wc -l a.txt
来源：http://ipr.jiagoushi.top

[R53] 查看文件头与实时尾
来源：http://omq.zhaomingkeji.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://awy.fktsv.cn

[R54] 比较两个文件
来源：http://xtr.yvedp.cn

diff a.txt b.txt
来源：http://vls.mhx1999.top

[R55] 压缩与解压
来源：http://ylf.hnxiangtu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nys.zhengqikj.top

[R56] 远程拷贝
来源：http://dsj.hywenlv.cn

scp file user@host:/path/
来源：http://jpm.dashuyun.cn

[R57] 远程执行命令
来源：http://aic.pycfn.com

ssh user@host 'uptime'
来源：http://uji.gogol.net.cn

[R58] 下载文件
来源：http://kdg.nanxuanxn.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jlo.ydjk.org.cn

[R59] 发 POST JSON
来源：http://joo.fanxiaobao.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iid.yj20258888.top

[R60] 只看 HTTP 状态码
来源：http://lne.cqqwz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mjp.52xcode.cn

[R61] 磁盘占用
来源：http://cik.cheryme.top

df -h;  du -sh *
来源：http://hyr.zdbjq.cn

[R62] 找最占空间的文件
来源：http://tay.havefunace.top

du -ah . | sort -rh | head -10
来源：http://vxn.gaohongyu789.top

[R63] 内存与进程
来源：http://zfq.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://qvl.vehdjk.com

[R64] 结束进程
来源：http://ehi.tianlin.xyz

kill -9 $(pgrep -f app.py)
来源：http://ile.hnqzz.top

[R65] 查看端口占用
来源：http://iro.jqgfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xwo.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://mie.zhaomingkeji.xyz

crontab -e;  crontab -l
来源：http://mgg.shuidangran.top

[R67] 生成随机十六进制串
来源：http://jkc.aibaodan.cn

openssl rand -hex 16
来源：http://lwg.quarkkingdee.top

[R68] 计算文件校验值
来源：http://opn.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://eii.jqgufenzy.top

[R69] 生成随机密码
来源：http://mrp.hcnkem.com

head -c 16 /dev/urandom | base64
来源：http://flk.tian-w.cn

[R70] 时间戳与互转
来源：http://kkn.feifeiyinyue.top

date +%s;  date -d @1700000000
来源：http://lle.shangyingyoupin.top

[R71] 日期格式化
来源：http://kak.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lrg.ydjk.org.cn

[R72] 等待端口就绪
来源：http://bha.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lru.havefunace.top

[R73] 分割大日志
来源：http://prb.epnwcf.com

split -l 1000 big.log part_
来源：http://mft.jyoumei.cn

[R74] 批量重命名
来源：http://ecl.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xgw.tian-w.cn

[R75] 导出环境变量
来源：http://fib.jinqigfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://xze.vehdjk.com

[R76] 使用临时文件
来源：http://rll.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rri.quarkkingdee.top

[R77] 读取用户输入
来源：http://wap.guannengcc.top

read -rp "请输入: " ans
来源：http://tdm.birdmap.top

[R78] 交互式菜单
来源：http://nql.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yar.bbcook.cn

[R79] 解析命令行选项
来源：http://pca.bbcook.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://afb.jqgfzy.top

[R80] 查看脚本执行耗时
来源：http://ilx.jianghu66.top

time ./run.sh
来源：http://yyh.kuanghao11.cn

================================================================================
来源：http://xhw.zhengqikj.top

S. C / C++ 专题
来源：http://pmi.yj20258.top

================================================================================
来源：http://rep.havefunace.top

[S01] C：Hello World
来源：http://gag.iojbl.cn

#include <stdio.h>
来源：http://obl.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ojp.fktsv.cn

[S02] C：变量与格式化输出
来源：http://wvj.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://gfn.sxryk.cn

[S03] C：读入整数
来源：http://dsy.havefunace.top

int x; scanf("%d", &x);
来源：http://mns.xylfe.cn

[S04] C：字符串复制
来源：http://ndc.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://eug.yuanzhike.top

[S05] C：字符串长度
来源：http://zel.gzhubu.top

strlen(s)
来源：http://iqb.redwolf501.top

[S06] C：字符串比较
来源：http://oil.nanxuanxn.top

strcmp(a, b) == 0
来源：http://yem.gotoacloud.top

[S07] C：数组遍历求和
来源：http://uri.kuanghao11.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mwq.hywenlv.cn

[S08] C：动态内存分配与释放
来源：http://rwc.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lhl.yueranfly.top

[S09] C：结构体定义与初始化
来源：http://yca.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rlg.0kj1m.cn

[S10] C：指针与解引用
来源：http://qlp.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://vmh.uphjek.com

[S11] C：逐行读文件
来源：http://zrv.gotoacloud.top

FILE *f = fopen("a.txt", "r");
来源：http://vte.guannengcc.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mbu.dashuyun.cn

fclose(f);
来源：http://wpv.ybcxt.top

[S12] C：写文件
来源：http://uma.aibaodan.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uer.chenlongwang.top

[S13] C：宏定义
来源：http://jha.birdmap.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qzp.smart0.xyz

[S14] C：枚举
来源：http://hmp.meibo888.top

enum Color { RED, GREEN, BLUE };
来源：http://bhz.cheryme.top

[S15] C：类型转换
来源：http://dkh.sysykeji.top

(double) a / b
来源：http://oek.shzxlz.cn

[S16] C：位操作置位
来源：http://gpm.9152youxi.cn

x |= (1 << 3);
来源：http://gwl.tanke756.top

[S17] C：安全拼接字符串
来源：http://woq.hongshengwenyu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hxg.haohaochexian.top

[S18] C：命令行参数
来源：http://wxj.zhongyouzk.top

int main(int argc, char **argv)
来源：http://wfb.shzxlz.cn

[S19] C：快速排序
来源：http://bpx.shanyushiyangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://lyg.ppjwa.cn

[S20] C：二分查找
来源：http://ihr.cdnleiting.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uhl.tian-w.cn

[S21] C：字符类别判断
来源：http://oym.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pao.pycfn.com

[S22] C：字符串转数字
来源：http://qhq.quarkkingdee.top

atoi("42");  strtod("3.14", NULL);
来源：http://tud.aibaodan.cn

[S23] C：随机数
来源：http://dqf.xinyue.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://akh.yvedp.cn

[S24] C：获取本地时间
来源：http://qxz.chenlongwang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bgp.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://tgg.yangfankeji.com

memcpy(dst, src, n);
来源：http://tjt.cashguo.top

[S26] C：内存清零
来源：http://vwf.shuidangran.top

memset(a, 0, sizeof a);
来源：http://pyn.shuidangran.top

[S27] C：定义常量
来源：http://wtj.pengpengdd.cyou

const double PI = 3.14159;
来源：http://lue.tanke756.top

[S28] C：静态变量
来源：http://fnm.wangdashe.top

static int counter = 0;
来源：http://ubl.hesvh.cn

[S29] C：变参函数
来源：http://vdp.shanyushiyangtech.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ciu.hcnkem.com

[S30] C：头文件保护
来源：http://reo.ydjk.org.cn

#ifndef X_H
来源：http://csb.epnwcf.com

#define X_H
来源：http://hyn.dashuyun.cn

#endif
来源：http://mor.jiagoushi.top

[S31] C++：Hello World
来源：http://xef.tarul.cn

#include <iostream>
来源：http://ymx.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://llg.tian-w.cn

[S32] C++：字符串
来源：http://mjo.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://afe.vehdjk.com

[S33] C++：vector 增删
来源：http://jzb.feifeiyinyue.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rkk.hammf.cn

[S34] C++：遍历 vector
来源：http://tvu.guannengcc.top

for (auto &x : v) { std::cout << x; }
来源：http://utf.svipenyu.cn

[S35] C++：map
来源：http://zpw.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jih.yuxming.cn

[S36] C++：unordered_map
来源：http://spn.ybcxt.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gmk.jianghu66.top

[S37] C++：set
来源：http://oly.yongpay.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kfe.iojbl.cn

[S38] C++：排序
来源：http://pef.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://ceh.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://kkj.shangyingyoupin.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wxe.gogol.net.cn

[S40] C++：查找元素
来源：http://wsc.ctjpmb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://stt.316326.xyz

[S41] C++：类与构造函数
来源：http://neq.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zwv.zhaomingkeji.xyz

[S42] C++：继承与虚函数
来源：http://nex.guowangkeji.top

class B : public Base { public: void f() override {} };
来源：http://eqi.shzxlz.cn

[S43] C++：智能指针
来源：http://clq.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://htc.shuidangran.top

[S44] C++：引用传参
来源：http://lnp.zhiwuduotai.top

void inc(int &x) { ++x; }
来源：http://zxw.snrcjt.cn

[S45] C++：lambda
来源：http://xen.zdbjq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://exj.havefunace.top

[S46] C++：函数模板
来源：http://ntc.yj202588.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lks.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://sie.yfazqb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blt.hnqzz.top

[S48] C++：逐行读文件
来源：http://jov.yuxming.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xzs.ydjk.org.cn

while (std::getline(in, line)) { }
来源：http://anx.svipenyu.cn

[S49] C++：写文件
来源：http://aec.ybcxt.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jhu.yj20258888.top

[S50] C++：格式化数字
来源：http://bni.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tja.hnqzz.top

[S51] C++：显式类型转换
来源：http://epz.jqgufenzy.top

static_cast<double>(a) / b
来源：http://wqg.snrcjt.cn

[S52] C++：const 与 noexcept
来源：http://gjf.pycfn.com


<!-- 参考信息 -->