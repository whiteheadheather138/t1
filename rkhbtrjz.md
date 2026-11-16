代发 wailian999

[Q84] 去除首尾空格
来源：http://zio.zhengqikj.top

SELECT TRIM(name) FROM users;
来源：http://got.pengpengdd.cyou

[Q85] 数值取整
来源：http://epj.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ilv.chenlongwang.top

[Q86] 读取 JSON 字段
来源：http://xwt.yj20258888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kzq.jinqigufen.top

[Q87] JSON 字段做条件
来源：http://ysh.tian-w.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pwu.gaohongyu789.top

[Q88] 行转列（条件聚合）
来源：http://ush.xuanzx.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zga.pengpengdd.cyou

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://geh.shzxlz.cn

[Q89] 判断表是否存在
来源：http://lsm.yongpay.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://men.daxiang520.top

[Q90] 生成序号列
来源：http://xnw.birdmap.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vna.xinyue.icu

================================================================================
来源：http://rtf.dianchejie.cn

R. Bash 专题
来源：http://hqy.chenzaomai.com

================================================================================
来源：http://beq.quarkkingdee.top

[R01] shebang 与严格模式
来源：http://ogt.xinyue.icu

#!/usr/bin/env bash
来源：http://lpr.zhaomingkeji.xyz

set -euo pipefail
来源：http://bww.xuetiantiany.cn

[R02] 变量赋值与使用
来源：http://ehn.wangdashe.top

name="Tom"; echo "$name"
来源：http://ffd.sweek.top

[R03] 只读变量
来源：http://bdm.andypj.xyz

readonly PI=3.14
来源：http://awv.xylfe.cn

[R04] 位置参数
来源：http://ytx.tianlin.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bqv.wangshuangyany.cn

[R05] 参数默认值
来源：http://nzn.gaohongyu789.top

name="${1:-default}"
来源：http://ebv.ywan-chungtsiang.top

[R06] 判断命令是否存在
来源：http://yjx.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jjx.shzxlz.cn

[R07] if 判断文件
来源：http://fhw.sweek.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zjt.xuetiantiany.cn

[R08] 数值比较
来源：http://rpa.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wce.meibo888.top

[R09] 字符串比较
来源：http://ytq.zhixingplan.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nka.svipenyu.cn

[R10] 正则匹配
来源：http://igp.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qtd.zhixingplan.top

[R11] case 多分支
来源：http://ccz.iojbl.cn

case "$1" in
来源：http://lns.yvedp.cn

start) echo "启动" ;;
来源：http://dlt.c1oappe.top

stop)  echo "停止" ;;
来源：http://vpn.daria6918.cn

*)     echo "未知命令" ;;
来源：http://egm.hammf.cn

esac
来源：http://aic.0kj1m.cn

[R12] for 遍历文件
来源：http://qsv.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://bak.nanxuanxn.top

[R13] for 计数循环
来源：http://exu.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://tvu.xingfuxueyuan.xyz

[R14] C 风格 for
来源：http://gmh.shanyushiyangtech.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mly.cdnleiting.top

[R15] while 逐行读文件
来源：http://xdy.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aat.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://wfm.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sfn.chenlongwang.top

[R17] 数组定义与取值
来源：http://ddc.smart0.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://uba.yj20258888.top

[R18] 遍历数组
来源：http://tdf.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jne.daxiang520.top

[R19] 数组长度
来源：http://lix.yj202588.top

echo "${#arr[@]}"
来源：http://tqn.aibaodan.cn

[R20] 关联数组（字典）
来源：http://ctl.yj20258.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wqq.jinqigufen.top

[R21] 字符串长度
来源：http://akn.iojbl.cn

echo "${#s}"
来源：http://fdr.zhongyouzk.top

[R22] 截取子串
来源：http://kjy.shzxlz.cn

echo "${s:0:5}"
来源：http://qpy.yonumen.top

[R23] 字符串替换
来源：http://lnz.hfpthk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xas.guannengcc.top

[R24] 大小写转换
来源：http://bbz.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://odz.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://ayb.sjlbkw.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://unu.shanyushiyangkeji.top

[R26] 命令替换
来源：http://jms.zhixingplan.top

now=$(date +%F); echo "$now"
来源：http://mlj.tanke756.top

[R27] 算术展开
来源：http://lqm.wangshuangyany.cn

echo $((1 + 2 * 3))
来源：http://fbq.0kj1m.cn

[R28] 浮点运算
来源：http://gto.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://cna.gzhubu.top

[R29] 定义函数
来源：http://aeu.zdqjudy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kdo.aibaodan.cn

[R30] 函数返回状态码
来源：http://ggz.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://uqk.kuanghao11.cn

[R31] 局部变量
来源：http://wnt.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://gqk.cashguo.top

[R32] 参数个数校验
来源：http://aio.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xdc.fktsv.cn

[R33] 捕获错误并提示行号
来源：http://rxs.kuanghao11.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ylh.andypj.xyz

[R34] 退出时清理
来源：http://ntt.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://pnq.cqqwz.cn

[R35] 后台执行并等待
来源：http://vxt.andypj.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ucd.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://fji.jqgufenzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tqr.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://cam.epnwcf.com

files=$(ls -1)
来源：http://hyu.fanxiaobao.xyz

[R38] 管道串联
来源：http://uxp.jinqigfzy.top

cat a.txt | grep -i error | wc -l
来源：http://frc.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://xga.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://scn.vqdsnc.cn

[R40] 追加写日志
来源：http://yfw.hongshengwenyu.top

echo "log" >> out.log
来源：http://kai.andypj.xyz

[R41] 丢弃输出
来源：http://jfg.zhixingplan.top

cmd >/dev/null 2>&1
来源：http://vku.redwolf501.top

[R42] 输入重定向
来源：http://ldt.fengsongda.top

wc -l < a.txt
来源：http://jey.yvedp.cn

[R43] 按名字查找文件
来源：http://aou.shzxlz.cn

find . -name "*.log" -type f
来源：http://etn.nanxuanxn.top

[R44] 按修改时间查找
来源：http://ihg.vehdjk.com

find . -mtime -7 -type f
来源：http://rqk.wangshuangyany.cn

[R45] 批量删除
来源：http://fni.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://mng.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://ynr.vehdjk.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ydh.fehbvm.com

[R47] sed 单行替换
来源：http://mfj.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dkf.316326.xyz

[R48] awk 取指定列
来源：http://vfb.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://yrd.xuanzx.com

[R49] awk 带条件
来源：http://shu.yvedp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vsf.xinyue.icu

[R50] awk 求和
来源：http://kge.jinyuanbaomall.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fzi.quarkkingdee.top

[R51] 排序去重取前几
来源：http://vwe.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://une.chenlongwang.top

[R52] 统计行数
来源：http://zwk.feifeiyinyue.top

wc -l a.txt
来源：http://roj.havefunace.top

[R53] 查看文件头与实时尾
来源：http://sob.daxiang520.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ezs.pengpengdd.cyou

[R54] 比较两个文件
来源：http://zsx.svipenyu.cn

diff a.txt b.txt
来源：http://jra.sweek.top

[R55] 压缩与解压
来源：http://guh.jinqigufen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ngi.sysykeji.top

[R56] 远程拷贝
来源：http://xcq.yueranfly.top

scp file user@host:/path/
来源：http://lpd.epnwcf.com

[R57] 远程执行命令
来源：http://nxo.tian-w.cn

ssh user@host 'uptime'
来源：http://knw.yonumen.top

[R58] 下载文件
来源：http://mcw.xylfe.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zyn.zhixingplan.top

[R59] 发 POST JSON
来源：http://ysg.haohaochexian.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vou.hesvh.cn

[R60] 只看 HTTP 状态码
来源：http://stv.xuetiantiany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zvc.chenzaomai.com

[R61] 磁盘占用
来源：http://fbo.zdqjudy.top

df -h;  du -sh *
来源：http://aze.hfpthk.cn

[R62] 找最占空间的文件
来源：http://fhz.ppjwa.cn

du -ah . | sort -rh | head -10
来源：http://jll.epnwcf.com

[R63] 内存与进程
来源：http://mhu.hammf.cn

free -h;  ps aux | grep nginx
来源：http://ihe.mhx1999.top

[R64] 结束进程
来源：http://mgt.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://fbn.sysykeji.top

[R65] 查看端口占用
来源：http://zht.feifeiyinyue.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zig.hnxiangtu.top

[R66] 定时任务
来源：http://dwg.fanxiaobao.xyz

crontab -e;  crontab -l
来源：http://ypo.ybcxt.top

[R67] 生成随机十六进制串
来源：http://eyu.fktsv.cn

openssl rand -hex 16
来源：http://yvf.yonumen.top

[R68] 计算文件校验值
来源：http://ito.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://okw.sweek.top

[R69] 生成随机密码
来源：http://yub.chenjidiqi.icu

head -c 16 /dev/urandom | base64
来源：http://pfc.52xcode.cn

[R70] 时间戳与互转
来源：http://dij.shangyingyoupin.top

date +%s;  date -d @1700000000
来源：http://euq.gogol.net.cn

[R71] 日期格式化
来源：http://aly.jianghu66.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bpz.birdmap.top

[R72] 等待端口就绪
来源：http://qxh.zdbjq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nnt.pycfn.com

[R73] 分割大日志
来源：http://hiv.jlsjyb.cn

split -l 1000 big.log part_
来源：http://qmd.hfpthk.cn

[R74] 批量重命名
来源：http://kvt.yangfankeji.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://omo.jinqigfzy.top

[R75] 导出环境变量
来源：http://nbc.ctjpmb.com

export PATH="$HOME/bin:$PATH"
来源：http://zbl.yuanzhike.top

[R76] 使用临时文件
来源：http://rmf.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xwm.tarul.cn

[R77] 读取用户输入
来源：http://quz.gogol.net.cn

read -rp "请输入: " ans
来源：http://ofc.epnwcf.com

[R78] 交互式菜单
来源：http://hpd.kuanghao11.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://efo.jyoumei.cn

[R79] 解析命令行选项
来源：http://rya.havefunace.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://poi.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://avm.hnxiangtu.top

time ./run.sh
来源：http://xvn.fehbvm.com

================================================================================
来源：http://omf.yj202588.top

S. C / C++ 专题
来源：http://trr.9152youxi.cn

================================================================================
来源：http://meg.sufxvd.cn

[S01] C：Hello World
来源：http://pkr.zdbjq.cn

#include <stdio.h>
来源：http://naf.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://qjz.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://xyh.xinyue.icu

int a = 10; printf("%d\n", a);
来源：http://etd.chenjidiqi.icu

[S03] C：读入整数
来源：http://oeg.9152youxi.cn

int x; scanf("%d", &x);
来源：http://mss.tanke756.top

[S04] C：字符串复制
来源：http://myb.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://hnh.tanke756.top

[S05] C：字符串长度
来源：http://xfu.hnxiangtu.top

strlen(s)
来源：http://ziu.hesvh.cn

[S06] C：字符串比较
来源：http://hbc.pycfn.com

strcmp(a, b) == 0
来源：http://iyf.redwolf501.top

[S07] C：数组遍历求和
来源：http://lzi.316326.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://reb.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://ysw.vehdjk.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xoz.zdqjudy.top

[S09] C：结构体定义与初始化
来源：http://rul.kuanghao11.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nwf.daria6918.cn

[S10] C：指针与解引用
来源：http://gov.mhx1999.top

int *p = &a;  *p = 5;
来源：http://vhi.wangdashe.top

[S11] C：逐行读文件
来源：http://vxx.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "r");
来源：http://lfx.chenlongwang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bnb.jqgufenzy.top

fclose(f);
来源：http://vgu.yangfankeji.com

[S12] C：写文件
来源：http://mur.zycfv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hjv.vehdjk.com

[S13] C：宏定义
来源：http://vkn.smart0.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fhm.sufxvd.cn

[S14] C：枚举
来源：http://hcn.316326.xyz

enum Color { RED, GREEN, BLUE };
来源：http://iju.aibaodan.cn

[S15] C：类型转换
来源：http://vdb.hnqzz.top

(double) a / b
来源：http://jkz.316326.xyz

[S16] C：位操作置位
来源：http://gss.snrcjt.cn

x |= (1 << 3);
来源：http://mok.yuxming.cn

[S17] C：安全拼接字符串
来源：http://kkl.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kkp.tarul.cn

[S18] C：命令行参数
来源：http://ejb.smart0.xyz

int main(int argc, char **argv)
来源：http://eef.pengpengdd.cyou

[S19] C：快速排序
来源：http://pti.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lxs.chenlongwang.top

[S20] C：二分查找
来源：http://mkl.feifeiyinyue.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tit.snrcjt.cn

[S21] C：字符类别判断
来源：http://qcm.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gbi.yanxiufei.cn

[S22] C：字符串转数字
来源：http://ved.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://thm.zhaomingkeji.xyz

[S23] C：随机数
来源：http://qmu.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lfz.hysaishi.cn

[S24] C：获取本地时间
来源：http://ljf.hywenlv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://igy.jinqigufen.top

[S25] C：内存拷贝
来源：http://vge.wangshuangyany.cn

memcpy(dst, src, n);
来源：http://xrg.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://hiy.xylfe.cn

memset(a, 0, sizeof a);
来源：http://ozf.ybcxt.top

[S27] C：定义常量
来源：http://bzk.gaohongyu789.top

const double PI = 3.14159;
来源：http://jlq.dashuyun.cn

[S28] C：静态变量
来源：http://znr.shanyushiyangtech.top

static int counter = 0;
来源：http://ugy.zhengqikj.top

[S29] C：变参函数
来源：http://fnl.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dwx.shuidangran.top

[S30] C：头文件保护
来源：http://iqp.pycfn.com

#ifndef X_H
来源：http://zim.yongpay.top

#define X_H
来源：http://tkc.xuetiantiany.cn

#endif
来源：http://eed.fktsv.cn

[S31] C++：Hello World
来源：http://xnt.52xcode.cn

#include <iostream>
来源：http://gij.redwolf501.top

int main() { std::cout << "Hello\n"; }
来源：http://zys.havefunace.top

[S32] C++：字符串
来源：http://dlr.0kj1m.cn

std::string s = "hi";  s += "!";
来源：http://epz.yueranfly.top

[S33] C++：vector 增删
来源：http://aob.xingfuxueyuan.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pnt.daxiang520.top

[S34] C++：遍历 vector
来源：http://lzq.guannengcc.top

for (auto &x : v) { std::cout << x; }
来源：http://xgg.ywan-chungtsiang.top

[S35] C++：map
来源：http://dhg.ybcxt.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uba.gotoacloud.top

[S36] C++：unordered_map
来源：http://wko.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wyt.sufxvd.cn

[S37] C++：set
来源：http://dye.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dlh.ybcxt.top

[S38] C++：排序
来源：http://dat.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://hcl.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://knc.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ifw.iojbl.cn

[S40] C++：查找元素
来源：http://pvk.zhongyouzk.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wmb.zhiwuduotai.top

[S41] C++：类与构造函数
来源：http://ykn.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bqo.xuetiantiany.cn

[S42] C++：继承与虚函数
来源：http://hvj.bjfxy.top

class B : public Base { public: void f() override {} };
来源：http://hoo.tianlin.xyz

[S43] C++：智能指针
来源：http://ijw.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://suo.mhx1999.top

[S44] C++：引用传参
来源：http://akj.mhx1999.top

void inc(int &x) { ++x; }
来源：http://nap.zdqjudy.top

[S45] C++：lambda
来源：http://ncc.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://iyw.hesvh.cn

[S46] C++：函数模板
来源：http://rgn.zhoulong.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jhv.dashuyun.cn

[S47] C++：结构化绑定遍历
来源：http://gze.quarkkingdee.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://urf.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://lsg.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pkj.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://tyx.c1oappe.top

[S49] C++：写文件
来源：http://reu.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wpa.yj202588.top

[S50] C++：格式化数字
来源：http://wxf.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lez.chenlongwang.top

[S51] C++：显式类型转换
来源：http://rqn.yongpay.top

static_cast<double>(a) / b
来源：http://dbi.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://grd.52xcode.cn

int size() const noexcept { return n_; }
来源：http://vxl.316326.xyz

[S53] C++：移动语义
来源：http://qja.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://wld.xuetiantiany.cn

[S54] C++：异常处理
来源：http://ecu.yanxiufei.cn


<!-- 参考信息 -->