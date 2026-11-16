代发 wailian999

[Q84] 去除首尾空格
来源：http://czf.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://scb.daxiang520.top

[Q85] 数值取整
来源：http://kut.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hqd.quarkkingdee.top

[Q86] 读取 JSON 字段
来源：http://yha.hnqzz.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://leq.xylfe.cn

[Q87] JSON 字段做条件
来源：http://gzt.redwolf501.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gwh.daxiang520.top

[Q88] 行转列（条件聚合）
来源：http://fjz.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tki.dianchejie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sjj.shangyingyoupin.top

[Q89] 判断表是否存在
来源：http://jan.jinghuilouyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ufq.hywenlv.cn

[Q90] 生成序号列
来源：http://qlf.gogol.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xwd.c1oappe.top

================================================================================
来源：http://ppg.jlsjyb.cn

R. Bash 专题
来源：http://scw.hywenlv.cn

================================================================================
来源：http://uqd.cashguo.top

[R01] shebang 与严格模式
来源：http://drz.fanxiaobao.xyz

#!/usr/bin/env bash
来源：http://yse.sufxvd.cn

set -euo pipefail
来源：http://eal.ydzc1.top

[R02] 变量赋值与使用
来源：http://alh.jinqigfzy.top

name="Tom"; echo "$name"
来源：http://ioz.yj202588.top

[R03] 只读变量
来源：http://wld.nanxuanxn.top

readonly PI=3.14
来源：http://pne.sysykeji.top

[R04] 位置参数
来源：http://uzx.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ees.zhixingplan.top

[R05] 参数默认值
来源：http://cyv.zhijiandao.cn

name="${1:-default}"
来源：http://rmy.ybcxt.top

[R06] 判断命令是否存在
来源：http://val.hongshengwenyu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://shq.shzxlz.cn

[R07] if 判断文件
来源：http://zbb.aibaodan.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qoh.ctjpmb.com

[R08] 数值比较
来源：http://izn.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gqs.hcnkem.com

[R09] 字符串比较
来源：http://fpo.yj202588.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://duj.fengsongda.top

[R10] 正则匹配
来源：http://xty.guannengcc.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ssp.cdnleiting.top

[R11] case 多分支
来源：http://loj.iojbl.cn

case "$1" in
来源：http://avy.zhaomingkeji.xyz

start) echo "启动" ;;
来源：http://lzx.sjlbkw.cn

stop)  echo "停止" ;;
来源：http://wms.jiagoushi.top

*)     echo "未知命令" ;;
来源：http://izh.ydzc1.top

esac
来源：http://wnv.jlsjyb.cn

[R12] for 遍历文件
来源：http://jjf.yj20258.top

for f in *.txt; do echo "$f"; done
来源：http://fkw.yongpay.top

[R13] for 计数循环
来源：http://awk.zhijiandao.cn

for i in {1..10}; do echo "$i"; done
来源：http://oep.chenjidiqi.icu

[R14] C 风格 for
来源：http://zbb.jqgufenzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iaw.shzxlz.cn

[R15] while 逐行读文件
来源：http://jaw.fengsongda.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rck.havefunace.top

[R16] until 等待条件
来源：http://hpv.uphjek.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rnk.jqgufenzy.top

[R17] 数组定义与取值
来源：http://xzw.dashuyun.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vmf.jiagoushi.top

[R18] 遍历数组
来源：http://zqo.vqdsnc.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ncj.aizwys.cn

[R19] 数组长度
来源：http://rfk.nanxuanxn.top

echo "${#arr[@]}"
来源：http://lav.hnqzz.top

[R20] 关联数组（字典）
来源：http://leq.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vhl.ybcxt.top

[R21] 字符串长度
来源：http://suk.zhiwuduotai.top

echo "${#s}"
来源：http://wab.nanxinkj.top

[R22] 截取子串
来源：http://fcq.yangfankeji.com

echo "${s:0:5}"
来源：http://rdb.guowangkeji.top

[R23] 字符串替换
来源：http://bmp.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jlg.yj20258.top

[R24] 大小写转换
来源：http://bqr.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://mji.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://tcm.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cvu.birdmap.top

[R26] 命令替换
来源：http://brx.yanxiufei.cn

now=$(date +%F); echo "$now"
来源：http://ijc.316326.xyz

[R27] 算术展开
来源：http://gzc.jqgfzy.top

echo $((1 + 2 * 3))
来源：http://nas.yueranfly.top

[R28] 浮点运算
来源：http://tog.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://sfl.hnxiangtu.top

[R29] 定义函数
来源：http://osi.ybcxt.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fsp.wangdashe.top

[R30] 函数返回状态码
来源：http://cbz.316326.xyz

f() { return 0; }; f || echo "失败了"
来源：http://jjl.yanxiufei.cn

[R31] 局部变量
来源：http://wfy.shuidangran.top

f() { local x=1; echo "$x"; }
来源：http://xea.feifeiyinyue.top

[R32] 参数个数校验
来源：http://vik.zhiwuduotai.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fyk.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://asg.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://soe.gaohongyu789.top

[R34] 退出时清理
来源：http://xvc.fehbvm.com

trap 'rm -f "$tmp"' EXIT
来源：http://mve.fzhhl.top

[R35] 后台执行并等待
来源：http://kut.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://erw.havefunace.top

[R36] 并发执行多个任务
来源：http://ogn.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jmg.ehwqpu.com

[R37] 把输出赋给变量
来源：http://jbp.gotoacloud.top

files=$(ls -1)
来源：http://pce.svipenyu.cn

[R38] 管道串联
来源：http://vkr.zycfv.cn

cat a.txt | grep -i error | wc -l
来源：http://uap.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://elg.yuxming.cn

cmd > out.log 2>&1
来源：http://hhe.cashguo.top

[R40] 追加写日志
来源：http://ful.nanxuanxn.top

echo "log" >> out.log
来源：http://nmf.jinghuilouyu.cn

[R41] 丢弃输出
来源：http://wsq.jqgfzy.top

cmd >/dev/null 2>&1
来源：http://ghn.yonumen.top

[R42] 输入重定向
来源：http://ejq.jinqigfzy.top

wc -l < a.txt
来源：http://cqm.kuanghao11.cn

[R43] 按名字查找文件
来源：http://acj.tianlin.xyz

find . -name "*.log" -type f
来源：http://znl.xziqi.cn

[R44] 按修改时间查找
来源：http://zef.tanke756.top

find . -mtime -7 -type f
来源：http://zbw.dashuyun.cn

[R45] 批量删除
来源：http://fjo.vehdjk.com

find . -name "*.tmp" -delete
来源：http://ukf.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://jim.yj20258888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kcw.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://lyd.mhx1999.top

sed -i 's/foo/bar/g' a.txt
来源：http://ijj.zhiwuduotai.top

[R48] awk 取指定列
来源：http://kwq.yuxming.cn

awk '{print $1, $3}' a.txt
来源：http://imp.svipenyu.cn

[R49] awk 带条件
来源：http://hhc.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nlp.uphjek.com

[R50] awk 求和
来源：http://kmq.ydjk.org.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nhl.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://wtz.yuanzhike.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hlz.sweek.top

[R52] 统计行数
来源：http://uqe.pengpengdd.cyou

wc -l a.txt
来源：http://caq.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://tsk.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://glt.tian-w.cn

[R54] 比较两个文件
来源：http://kkt.xingfuxueyuan.xyz

diff a.txt b.txt
来源：http://fho.yvedp.cn

[R55] 压缩与解压
来源：http://gpu.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cea.dianchejie.cn

[R56] 远程拷贝
来源：http://ssd.ivvv.top

scp file user@host:/path/
来源：http://ryj.andypj.xyz

[R57] 远程执行命令
来源：http://vty.yanxiufei.cn

ssh user@host 'uptime'
来源：http://ppf.yvedp.cn

[R58] 下载文件
来源：http://suh.c1oappe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ogn.fengsongda.top

[R59] 发 POST JSON
来源：http://xmg.bjfxy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://itv.epnwcf.com

[R60] 只看 HTTP 状态码
来源：http://jme.jinqigufen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fkh.tarul.cn

[R61] 磁盘占用
来源：http://pri.feifeiyinyue.top

df -h;  du -sh *
来源：http://ygx.bjfxy.top

[R62] 找最占空间的文件
来源：http://sfb.hesvh.cn

du -ah . | sort -rh | head -10
来源：http://ojv.yj20258.top

[R63] 内存与进程
来源：http://bxw.ivvv.top

free -h;  ps aux | grep nginx
来源：http://nwq.svipenyu.cn

[R64] 结束进程
来源：http://tli.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://bkt.chenzaomai.com

[R65] 查看端口占用
来源：http://dmy.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pmf.vehdjk.com

[R66] 定时任务
来源：http://phs.fktsv.cn

crontab -e;  crontab -l
来源：http://xor.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://kjp.ydzc1.top

openssl rand -hex 16
来源：http://wqm.ywan-chungtsiang.top

[R68] 计算文件校验值
来源：http://jtf.chenzaomai.com

sha256sum a.txt;  md5sum a.txt
来源：http://efi.zhixingplan.top

[R69] 生成随机密码
来源：http://fbt.mhx1999.top

head -c 16 /dev/urandom | base64
来源：http://ofc.ppjwa.cn

[R70] 时间戳与互转
来源：http://kup.jqgfzy.top

date +%s;  date -d @1700000000
来源：http://rmr.chenjidiqi.icu

[R71] 日期格式化
来源：http://bfl.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dva.shanyushiyangkeji.top

[R72] 等待端口就绪
来源：http://ful.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rfa.hammf.cn

[R73] 分割大日志
来源：http://wvm.redwolf501.top

split -l 1000 big.log part_
来源：http://sbe.quarkkingdee.top

[R74] 批量重命名
来源：http://gbb.yj20258.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bqu.zhongyouzk.top

[R75] 导出环境变量
来源：http://koj.bjfxy.top

export PATH="$HOME/bin:$PATH"
来源：http://mna.xylfe.cn

[R76] 使用临时文件
来源：http://gyt.zdqjudy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://slv.xylfe.cn

[R77] 读取用户输入
来源：http://foz.sweek.top

read -rp "请输入: " ans
来源：http://nqc.hongshengwenyu.top

[R78] 交互式菜单
来源：http://qrj.fehbvm.com

select opt in a b c; do echo "$opt"; break; done
来源：http://yuv.tanke756.top

[R79] 解析命令行选项
来源：http://mfc.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sas.fktsv.cn

[R80] 查看脚本执行耗时
来源：http://clu.jiagoushi.top

time ./run.sh
来源：http://wat.daxiang520.top

================================================================================
来源：http://jbq.yvedp.cn

S. C / C++ 专题
来源：http://tro.hongshengwenyu.top

================================================================================
来源：http://woo.sufxvd.cn

[S01] C：Hello World
来源：http://qgq.hesvh.cn

#include <stdio.h>
来源：http://zcm.fehbvm.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://blj.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://tbr.ywan-chungtsiang.top

int a = 10; printf("%d\n", a);
来源：http://ugh.ydjk.org.cn

[S03] C：读入整数
来源：http://jfn.gogol.net.cn

int x; scanf("%d", &x);
来源：http://iow.316326.xyz

[S04] C：字符串复制
来源：http://kek.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://jmj.cqqwz.cn

[S05] C：字符串长度
来源：http://wym.zhixingplan.top

strlen(s)
来源：http://cqo.xziqi.cn

[S06] C：字符串比较
来源：http://nzw.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://xns.jinqigufen.top

[S07] C：数组遍历求和
来源：http://zby.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xml.0kj1m.cn

[S08] C：动态内存分配与释放
来源：http://rmn.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nzt.ydzc1.top

[S09] C：结构体定义与初始化
来源：http://tje.yanxiufei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://glb.zhoulong.xyz

[S10] C：指针与解引用
来源：http://ibf.daxiang520.top

int *p = &a;  *p = 5;
来源：http://dvz.jiagoushi.top

[S11] C：逐行读文件
来源：http://qka.sweek.top

FILE *f = fopen("a.txt", "r");
来源：http://ajj.yonumen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cdc.wangshuangyany.cn

fclose(f);
来源：http://bbu.ivvv.top

[S12] C：写文件
来源：http://bzj.bbcook.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xga.jinghuilouyu.cn

[S13] C：宏定义
来源：http://qok.zhixingplan.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ion.gaohongyu789.top

[S14] C：枚举
来源：http://zju.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://bfk.cucudq.cn

[S15] C：类型转换
来源：http://vph.mhx1999.top

(double) a / b
来源：http://wov.yonumen.top

[S16] C：位操作置位
来源：http://fcr.hammf.cn

x |= (1 << 3);
来源：http://vdf.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://tjx.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lya.pengpengdd.cyou

[S18] C：命令行参数
来源：http://rbr.hysaishi.cn

int main(int argc, char **argv)
来源：http://osi.zhixingplan.top

[S19] C：快速排序
来源：http://slk.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://tng.snrcjt.cn

[S20] C：二分查找
来源：http://aeg.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sov.iojbl.cn

[S21] C：字符类别判断
来源：http://lyp.sjlbkw.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eal.52xcode.cn

[S22] C：字符串转数字
来源：http://hez.iojbl.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zjy.fktsv.cn

[S23] C：随机数
来源：http://qlw.hnxiangtu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xxx.smart0.xyz

[S24] C：获取本地时间
来源：http://rpj.sysykeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://opz.epnwcf.com

[S25] C：内存拷贝
来源：http://lwg.sjlbkw.cn

memcpy(dst, src, n);
来源：http://zyz.jinqigufen.top

[S26] C：内存清零
来源：http://pfu.yanxiufei.cn

memset(a, 0, sizeof a);
来源：http://bzz.xingfuxueyuan.xyz

[S27] C：定义常量
来源：http://rxv.ydjk.org.cn

const double PI = 3.14159;
来源：http://rqx.redwolf501.top

[S28] C：静态变量
来源：http://mcu.yanxiufei.cn

static int counter = 0;
来源：http://opj.sysykeji.top

[S29] C：变参函数
来源：http://dgk.vqdsnc.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dvz.cashguo.top

[S30] C：头文件保护
来源：http://aje.zhiwuduotai.top

#ifndef X_H
来源：http://dtr.fengsongda.top

#define X_H
来源：http://bkd.gzhubu.top

#endif
来源：http://xno.jlsjyb.cn

[S31] C++：Hello World
来源：http://sug.sweek.top

#include <iostream>
来源：http://tpy.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://wgp.52xcode.cn

[S32] C++：字符串
来源：http://vds.jinqigufen.top

std::string s = "hi";  s += "!";
来源：http://wxx.yangfankeji.com

[S33] C++：vector 增删
来源：http://ded.316326.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gyv.sysykeji.top

[S34] C++：遍历 vector
来源：http://ssj.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://tec.jinqigufen.top

[S35] C++：map
来源：http://mpd.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dyj.mhx1999.top

[S36] C++：unordered_map
来源：http://tqi.cqqwz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://clc.zhongyouzk.top

[S37] C++：set
来源：http://ehs.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ekw.yangfankeji.com

[S38] C++：排序
来源：http://oxq.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://ngb.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://rbl.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hxl.yongpay.top

[S40] C++：查找元素
来源：http://uyr.nanxinkj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zxu.xingfuxueyuan.xyz

[S41] C++：类与构造函数
来源：http://cfr.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mfn.gzhubu.top

[S42] C++：继承与虚函数
来源：http://tgb.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://npl.svipenyu.cn

[S43] C++：智能指针
来源：http://eci.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://duj.aibaodan.cn

[S44] C++：引用传参
来源：http://abo.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://adc.gotoacloud.top

[S45] C++：lambda
来源：http://hxn.yongpay.top

auto add = [](int a, int b) { return a + b; };
来源：http://iqo.fktsv.cn

[S46] C++：函数模板
来源：http://brz.wangdashe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eyb.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://anv.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lhl.xziqi.cn

[S48] C++：逐行读文件
来源：http://mby.vehdjk.com

std::ifstream in("a.txt");  std::string line;
来源：http://rri.andypj.xyz

while (std::getline(in, line)) { }
来源：http://aoz.daria6918.cn

[S49] C++：写文件
来源：http://lhl.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ymw.bjfxy.top

[S50] C++：格式化数字
来源：http://djf.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uha.ehwqpu.com

[S51] C++：显式类型转换
来源：http://yne.vehdjk.com

static_cast<double>(a) / b
来源：http://ufc.316326.xyz

[S52] C++：const 与 noexcept
来源：http://zgq.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://jol.xuetiantiany.cn

[S53] C++：移动语义
来源：http://dfy.bbcook.cn

std::vector<int> w = std::move(v);
来源：http://jdi.feifeiyinyue.top

[S54] C++：异常处理
来源：http://xay.aizwys.cn


<!-- 参考信息 -->