代发 wailian999

[Q82] 字符长度与字节长度
来源：http://uoq.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xbt.xuanzx.com

[Q83] 大小写转换
来源：http://xkv.shanyushiyangtech.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tsv.chenjidiqi.icu

[Q84] 去除首尾空格
来源：http://ntp.jlsjyb.cn

SELECT TRIM(name) FROM users;
来源：http://qxn.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://ozh.cucudq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eya.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://frp.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kdu.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://bhb.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://med.tianlin.xyz

[Q88] 行转列（条件聚合）
来源：http://etz.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lvc.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kzo.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://kjb.zhongyouzk.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pfd.bjfxy.top

[Q90] 生成序号列
来源：http://cla.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dlu.nanxinkj.top

================================================================================
来源：http://qla.nanxinkj.top

R. Bash 专题
来源：http://buq.9152youxi.cn

================================================================================
来源：http://cax.yuanzhike.top

[R01] shebang 与严格模式
来源：http://iyy.bjfxy.top

#!/usr/bin/env bash
来源：http://vbt.zdqjudy.top

set -euo pipefail
来源：http://ier.hongshengwenyu.top

[R02] 变量赋值与使用
来源：http://mdf.hywenlv.cn

name="Tom"; echo "$name"
来源：http://ugl.hysaishi.cn

[R03] 只读变量
来源：http://ojs.jinqigfzy.top

readonly PI=3.14
来源：http://wjx.xinyue.icu

[R04] 位置参数
来源：http://otz.9152youxi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kcw.gotoacloud.top

[R05] 参数默认值
来源：http://poi.yueranfly.top

name="${1:-default}"
来源：http://ikc.pycfn.com

[R06] 判断命令是否存在
来源：http://wvt.smart0.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qye.ctjpmb.com

[R07] if 判断文件
来源：http://fuy.yfazqb.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pci.bjfxy.top

[R08] 数值比较
来源：http://rfj.yueranfly.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gey.yongpay.top

[R09] 字符串比较
来源：http://dxp.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xvo.daria6918.cn

[R10] 正则匹配
来源：http://arq.yueranfly.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nra.fengsongda.top

[R11] case 多分支
来源：http://iii.chenzaomai.com

case "$1" in
来源：http://dmo.wangshuangyany.cn

start) echo "启动" ;;
来源：http://djf.ivvv.top

stop)  echo "停止" ;;
来源：http://dsl.xinyue.icu

*)     echo "未知命令" ;;
来源：http://ibf.yanxiufei.cn

esac
来源：http://muc.ehwqpu.com

[R12] for 遍历文件
来源：http://vwj.ywan-chungtsiang.top

for f in *.txt; do echo "$f"; done
来源：http://opw.andypj.xyz

[R13] for 计数循环
来源：http://gcc.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://aap.pengpengdd.cyou

[R14] C 风格 for
来源：http://yki.9152youxi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eme.hnxiangtu.top

[R15] while 逐行读文件
来源：http://nfm.dianchejie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cgo.tanke756.top

[R16] until 等待条件
来源：http://joz.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qfh.yj202588.top

[R17] 数组定义与取值
来源：http://tqa.shzxlz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wdt.tianlin.xyz

[R18] 遍历数组
来源：http://igw.daxiang520.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nqj.jinqigfzy.top

[R19] 数组长度
来源：http://jwu.hesvh.cn

echo "${#arr[@]}"
来源：http://owy.xinyue.icu

[R20] 关联数组（字典）
来源：http://kmh.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vnw.birdmap.top

[R21] 字符串长度
来源：http://bkl.sysykeji.top

echo "${#s}"
来源：http://qby.52xcode.cn

[R22] 截取子串
来源：http://zud.hesvh.cn

echo "${s:0:5}"
来源：http://ibc.wangdashe.top

[R23] 字符串替换
来源：http://wti.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vld.jinyuanbaomall.cn

[R24] 大小写转换
来源：http://fiy.9152youxi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://exf.aibaodan.cn

[R25] 去后缀 / 去前缀
来源：http://hld.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xza.9152youxi.cn

[R26] 命令替换
来源：http://puh.zdbjq.cn

now=$(date +%F); echo "$now"
来源：http://keb.fehbvm.com

[R27] 算术展开
来源：http://jqv.ydjk.org.cn

echo $((1 + 2 * 3))
来源：http://lcg.guannengcc.top

[R28] 浮点运算
来源：http://kaa.shuidangran.top

echo "scale=2; 10/3" | bc
来源：http://fgv.zhengqikj.top

[R29] 定义函数
来源：http://wph.aizwys.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cht.yfazqb.com

[R30] 函数返回状态码
来源：http://wwv.ydzc1.top

f() { return 0; }; f || echo "失败了"
来源：http://fhi.316326.xyz

[R31] 局部变量
来源：http://oeh.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://zmt.zhongyouzk.top

[R32] 参数个数校验
来源：http://cta.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dpg.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://gli.jinyuanbaomall.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kgy.zdbjq.cn

[R34] 退出时清理
来源：http://vmd.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://ofo.zdqjudy.top

[R35] 后台执行并等待
来源：http://wzh.daria6918.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hwm.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://yid.xuanzx.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fmv.guowangkeji.top

[R37] 把输出赋给变量
来源：http://sct.quarkkingdee.top

files=$(ls -1)
来源：http://xot.fzhhl.top

[R38] 管道串联
来源：http://oyr.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://fza.shangyingyoupin.top

[R39] 重定向标准输出与错误
来源：http://zcy.hcnkem.com

cmd > out.log 2>&1
来源：http://cum.svipenyu.cn

[R40] 追加写日志
来源：http://acq.hfpthk.cn

echo "log" >> out.log
来源：http://fib.vqdsnc.cn

[R41] 丢弃输出
来源：http://znc.jlsjyb.cn

cmd >/dev/null 2>&1
来源：http://djr.yuanzhike.top

[R42] 输入重定向
来源：http://dez.cqqwz.cn

wc -l < a.txt
来源：http://qxw.ydjk.org.cn

[R43] 按名字查找文件
来源：http://zou.tianlin.xyz

find . -name "*.log" -type f
来源：http://hmn.birdmap.top

[R44] 按修改时间查找
来源：http://qao.tian-w.cn

find . -mtime -7 -type f
来源：http://yng.svipenyu.cn

[R45] 批量删除
来源：http://xxd.xylfe.cn

find . -name "*.tmp" -delete
来源：http://bck.yvedp.cn

[R46] 递归替换文件内容
来源：http://umv.jqgufenzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nzy.cashguo.top

[R47] sed 单行替换
来源：http://gon.tian-w.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ter.chenzaomai.com

[R48] awk 取指定列
来源：http://nwl.ppjwa.cn

awk '{print $1, $3}' a.txt
来源：http://bte.tarul.cn

[R49] awk 带条件
来源：http://xig.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ban.hcnkem.com

[R50] awk 求和
来源：http://dkq.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kpb.cucudq.cn

[R51] 排序去重取前几
来源：http://yva.tanke756.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ubt.jinqigfzy.top

[R52] 统计行数
来源：http://djv.bjfxy.top

wc -l a.txt
来源：http://the.mhx1999.top

[R53] 查看文件头与实时尾
来源：http://zmi.bbcook.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aji.ppjwa.cn

[R54] 比较两个文件
来源：http://gsr.yj202588.top

diff a.txt b.txt
来源：http://mvm.sysykeji.top

[R55] 压缩与解压
来源：http://jxe.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bms.zhixingplan.top

[R56] 远程拷贝
来源：http://bcx.guowangkeji.top

scp file user@host:/path/
来源：http://orv.xinyue.icu

[R57] 远程执行命令
来源：http://cgg.yongpay.top

ssh user@host 'uptime'
来源：http://suq.nwbrower.top

[R58] 下载文件
来源：http://xqu.birdmap.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://znn.sweek.top

[R59] 发 POST JSON
来源：http://yhy.xingfuxueyuan.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ypr.hongshengwenyu.top

[R60] 只看 HTTP 状态码
来源：http://xsc.svipenyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fah.c1oappe.top

[R61] 磁盘占用
来源：http://fdk.tianlin.xyz

df -h;  du -sh *
来源：http://yip.tianlin.xyz

[R62] 找最占空间的文件
来源：http://dtx.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://xin.snrcjt.cn

[R63] 内存与进程
来源：http://gnc.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://kal.chenlongwang.top

[R64] 结束进程
来源：http://hkd.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://rwt.c1oappe.top

[R65] 查看端口占用
来源：http://yky.hongshengwenyu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vvh.yuanzhike.top

[R66] 定时任务
来源：http://jop.gaohongyu789.top

crontab -e;  crontab -l
来源：http://wtj.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://gak.sjlbkw.cn

openssl rand -hex 16
来源：http://ofv.jqgfzy.top

[R68] 计算文件校验值
来源：http://bvk.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fjc.xuanzx.com

[R69] 生成随机密码
来源：http://urz.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://lcn.jqgufenzy.top

[R70] 时间戳与互转
来源：http://oqf.ehwqpu.com

date +%s;  date -d @1700000000
来源：http://wzr.hysaishi.cn

[R71] 日期格式化
来源：http://bzr.jinyuanbaomall.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ocv.c1oappe.top

[R72] 等待端口就绪
来源：http://mie.ctjpmb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://nud.iojbl.cn

[R73] 分割大日志
来源：http://zgj.svipenyu.cn

split -l 1000 big.log part_
来源：http://kfp.cdnleiting.top

[R74] 批量重命名
来源：http://neg.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kdm.birdmap.top

[R75] 导出环境变量
来源：http://erm.yfazqb.com

export PATH="$HOME/bin:$PATH"
来源：http://sfv.0kj1m.cn

[R76] 使用临时文件
来源：http://zoa.yj20258888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://htd.smart0.xyz

[R77] 读取用户输入
来源：http://hce.smart0.xyz

read -rp "请输入: " ans
来源：http://uwu.yuxming.cn

[R78] 交互式菜单
来源：http://ayz.meibo888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ngp.fzhhl.top

[R79] 解析命令行选项
来源：http://pyb.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gpl.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://mrb.jlsjyb.cn

time ./run.sh
来源：http://xes.jianghu66.top

================================================================================
来源：http://feb.guannengcc.top

S. C / C++ 专题
来源：http://pcv.jqgfzy.top

================================================================================
来源：http://kmn.fktsv.cn

[S01] C：Hello World
来源：http://ytn.zhongyouzk.top

#include <stdio.h>
来源：http://hui.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://hmp.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://gge.ppjwa.cn

int a = 10; printf("%d\n", a);
来源：http://xcj.zhoulong.xyz

[S03] C：读入整数
来源：http://blt.nwbrower.top

int x; scanf("%d", &x);
来源：http://zja.sxryk.cn

[S04] C：字符串复制
来源：http://rqk.zhoulong.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://fiv.zhaomingkeji.xyz

[S05] C：字符串长度
来源：http://mgt.andypj.xyz

strlen(s)
来源：http://fct.ppjwa.cn

[S06] C：字符串比较
来源：http://gza.nanxuanxn.top

strcmp(a, b) == 0
来源：http://efh.pengpengdd.cyou

[S07] C：数组遍历求和
来源：http://eyo.gogol.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zbt.daxiang520.top

[S08] C：动态内存分配与释放
来源：http://bel.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jcs.fktsv.cn

[S09] C：结构体定义与初始化
来源：http://bak.yj20258.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://thj.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://wzc.yj20258888.top

int *p = &a;  *p = 5;
来源：http://xic.hnxiangtu.top

[S11] C：逐行读文件
来源：http://kja.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://frj.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://jsl.52xcode.cn

fclose(f);
来源：http://ewe.jinqigfzy.top

[S12] C：写文件
来源：http://uqx.xziqi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ehh.smart0.xyz

[S13] C：宏定义
来源：http://tre.316326.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aom.andypj.xyz

[S14] C：枚举
来源：http://mgl.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://mfb.jinyuanbaomall.cn

[S15] C：类型转换
来源：http://nro.andypj.xyz

(double) a / b
来源：http://hpi.hongshengwenyu.top

[S16] C：位操作置位
来源：http://bnw.jinyuanbaomall.cn

x |= (1 << 3);
来源：http://lqg.pengpengdd.cyou

[S17] C：安全拼接字符串
来源：http://kun.nanxinkj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uwy.xuanzx.com

[S18] C：命令行参数
来源：http://str.yonumen.top

int main(int argc, char **argv)
来源：http://mvg.xinyue.icu

[S19] C：快速排序
来源：http://ijv.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ief.sweek.top

[S20] C：二分查找
来源：http://wst.sysykeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vor.dianchejie.cn

[S21] C：字符类别判断
来源：http://yts.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vvz.yanxiufei.cn

[S22] C：字符串转数字
来源：http://dzx.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uwm.aizwys.cn

[S23] C：随机数
来源：http://tcg.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jpg.zhengqikj.top

[S24] C：获取本地时间
来源：http://ffp.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qhw.fzhhl.top

[S25] C：内存拷贝
来源：http://nsd.guannengcc.top

memcpy(dst, src, n);
来源：http://ghf.smart0.xyz

[S26] C：内存清零
来源：http://phz.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://mqn.ehwqpu.com

[S27] C：定义常量
来源：http://ses.yonumen.top

const double PI = 3.14159;
来源：http://mnc.fzhhl.top

[S28] C：静态变量
来源：http://tjt.zycfv.cn

static int counter = 0;
来源：http://bfl.hywenlv.cn

[S29] C：变参函数
来源：http://qyb.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://urf.fengsongda.top

[S30] C：头文件保护
来源：http://fmu.pycfn.com

#ifndef X_H
来源：http://dpn.snrcjt.cn

#define X_H
来源：http://vnf.birdmap.top

#endif
来源：http://tyx.daxiang520.top

[S31] C++：Hello World
来源：http://wky.nanxuanxn.top

#include <iostream>
来源：http://ool.ybcxt.top

int main() { std::cout << "Hello\n"; }
来源：http://dmi.nwbrower.top

[S32] C++：字符串
来源：http://atj.dashuyun.cn

std::string s = "hi";  s += "!";
来源：http://yel.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://byx.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fxj.redwolf501.top

[S34] C++：遍历 vector
来源：http://udd.jqgufenzy.top

for (auto &x : v) { std::cout << x; }
来源：http://fan.gotoacloud.top

[S35] C++：map
来源：http://fyd.jianghu66.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wfx.uphjek.com

[S36] C++：unordered_map
来源：http://jbp.ywan-chungtsiang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lrb.hcnkem.com

[S37] C++：set
来源：http://nnn.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wqn.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://ris.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://wgg.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://hck.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dol.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://ruy.vqdsnc.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vte.yuanzhike.top

[S41] C++：类与构造函数
来源：http://zaw.yuanzhike.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tsv.tarul.cn

[S42] C++：继承与虚函数
来源：http://akp.yuanzhike.top

class B : public Base { public: void f() override {} };
来源：http://ehm.xinyue.icu

[S43] C++：智能指针
来源：http://vkr.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://str.cheryme.top

[S44] C++：引用传参
来源：http://mrk.gzhubu.top

void inc(int &x) { ++x; }
来源：http://jkp.sufxvd.cn

[S45] C++：lambda
来源：http://bes.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hjv.fehbvm.com

[S46] C++：函数模板
来源：http://jcu.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dco.zhoulong.xyz

[S47] C++：结构化绑定遍历
来源：http://vmu.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://som.ydzc1.top

[S48] C++：逐行读文件
来源：http://gnd.xinyue.icu

std::ifstream in("a.txt");  std::string line;
来源：http://znp.jinqigfzy.top

while (std::getline(in, line)) { }
来源：http://dmb.zycfv.cn

[S49] C++：写文件
来源：http://brf.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sel.0kj1m.cn

[S50] C++：格式化数字
来源：http://jks.shzxlz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jvj.xziqi.cn

[S51] C++：显式类型转换
来源：http://knw.cqqwz.cn

static_cast<double>(a) / b
来源：http://rwm.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://adu.sysykeji.top


<!-- 参考信息 -->