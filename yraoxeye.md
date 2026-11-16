代发 wailian999

[Q80] 字符串截取
来源：http://hyr.jinqigfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ydy.sysykeji.top

[Q81] 字符串替换
来源：http://pgf.cdnleiting.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yig.yvedp.cn

[Q82] 字符长度与字节长度
来源：http://udo.hammf.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ngm.xziqi.cn

[Q83] 大小写转换
来源：http://ozi.chenjidiqi.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rre.zycfv.cn

[Q84] 去除首尾空格
来源：http://elf.yj20258888.top

SELECT TRIM(name) FROM users;
来源：http://bfh.zhixingplan.top

[Q85] 数值取整
来源：http://fqv.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mpk.jiagoushi.top

[Q86] 读取 JSON 字段
来源：http://zto.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wgx.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://pss.gogol.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pyh.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://fuu.yj20258.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pkx.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://axv.ctjpmb.com

[Q89] 判断表是否存在
来源：http://jai.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sxc.vqdsnc.cn

[Q90] 生成序号列
来源：http://bwy.zycfv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fym.uphjek.com

================================================================================
来源：http://pkp.zhoulong.xyz

R. Bash 专题
来源：http://ywn.jinqigufen.top

================================================================================
来源：http://gej.wangdashe.top

[R01] shebang 与严格模式
来源：http://zat.cqqwz.cn

#!/usr/bin/env bash
来源：http://idn.zhengqikj.top

set -euo pipefail
来源：http://cna.vehdjk.com

[R02] 变量赋值与使用
来源：http://tjg.jianghu66.top

name="Tom"; echo "$name"
来源：http://jsy.jianghu66.top

[R03] 只读变量
来源：http://gci.wangshuangyany.cn

readonly PI=3.14
来源：http://qcf.havefunace.top

[R04] 位置参数
来源：http://lpi.tarul.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dgt.wangshuangyany.cn

[R05] 参数默认值
来源：http://kvf.jyoumei.cn

name="${1:-default}"
来源：http://ayb.fehbvm.com

[R06] 判断命令是否存在
来源：http://nxb.shanyushiyangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xfu.bbcook.cn

[R07] if 判断文件
来源：http://rxu.sufxvd.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nbl.sweek.top

[R08] 数值比较
来源：http://rxm.jqgfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cyn.nwbrower.top

[R09] 字符串比较
来源：http://xpe.tian-w.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ulw.jlsjyb.cn

[R10] 正则匹配
来源：http://pbj.yonumen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bog.nanxuanxn.top

[R11] case 多分支
来源：http://mcs.bjfxy.top

case "$1" in
来源：http://sbb.ivvv.top

start) echo "启动" ;;
来源：http://tyc.xziqi.cn

stop)  echo "停止" ;;
来源：http://pfk.yfazqb.com

*)     echo "未知命令" ;;
来源：http://iiz.jinqigfzy.top

esac
来源：http://cvx.fktsv.cn

[R12] for 遍历文件
来源：http://jen.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://xux.snrcjt.cn

[R13] for 计数循环
来源：http://eno.chenlongwang.top

for i in {1..10}; do echo "$i"; done
来源：http://avw.cqqwz.cn

[R14] C 风格 for
来源：http://gkw.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tkb.haohaochexian.top

[R15] while 逐行读文件
来源：http://dug.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qpz.dianchejie.cn

[R16] until 等待条件
来源：http://edd.haohaochexian.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ztf.cucudq.cn

[R17] 数组定义与取值
来源：http://six.bjfxy.top

arr=(a b c); echo "${arr[0]}"
来源：http://woe.sufxvd.cn

[R18] 遍历数组
来源：http://xls.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hte.svipenyu.cn

[R19] 数组长度
来源：http://epz.zhixingplan.top

echo "${#arr[@]}"
来源：http://wrz.wangshuangyany.cn

[R20] 关联数组（字典）
来源：http://rdr.cucudq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qfk.jlsjyb.cn

[R21] 字符串长度
来源：http://hps.yangfankeji.com

echo "${#s}"
来源：http://ema.jinghuilouyu.cn

[R22] 截取子串
来源：http://yya.bbcook.cn

echo "${s:0:5}"
来源：http://uuj.hywenlv.cn

[R23] 字符串替换
来源：http://udd.zhiwuduotai.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nol.ydzc1.top

[R24] 大小写转换
来源：http://lon.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://jxx.mhx1999.top

[R25] 去后缀 / 去前缀
来源：http://pat.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xmc.mhx1999.top

[R26] 命令替换
来源：http://uma.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://wis.xylfe.cn

[R27] 算术展开
来源：http://jwa.ehwqpu.com

echo $((1 + 2 * 3))
来源：http://swe.yongpay.top

[R28] 浮点运算
来源：http://vsz.sufxvd.cn

echo "scale=2; 10/3" | bc
来源：http://aov.tian-w.cn

[R29] 定义函数
来源：http://uxg.kuanghao11.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xxl.yuxming.cn

[R30] 函数返回状态码
来源：http://cba.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://sxm.tianlin.xyz

[R31] 局部变量
来源：http://woe.fehbvm.com

f() { local x=1; echo "$x"; }
来源：http://tfb.hammf.cn

[R32] 参数个数校验
来源：http://jyc.yvedp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gmn.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://cbq.nwbrower.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bht.hywenlv.cn

[R34] 退出时清理
来源：http://kcs.yongpay.top

trap 'rm -f "$tmp"' EXIT
来源：http://cyt.haohaochexian.top

[R35] 后台执行并等待
来源：http://cuk.andypj.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://sit.yongpay.top

[R36] 并发执行多个任务
来源：http://sjj.tarul.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dwq.aibaodan.cn

[R37] 把输出赋给变量
来源：http://qee.quarkkingdee.top

files=$(ls -1)
来源：http://hjm.yanxiufei.cn

[R38] 管道串联
来源：http://jgf.fanxiaobao.xyz

cat a.txt | grep -i error | wc -l
来源：http://sqb.zhixingplan.top

[R39] 重定向标准输出与错误
来源：http://wyi.sweek.top

cmd > out.log 2>&1
来源：http://lnh.iojbl.cn

[R40] 追加写日志
来源：http://umo.nanxinkj.top

echo "log" >> out.log
来源：http://zyi.jinyuanbaomall.cn

[R41] 丢弃输出
来源：http://cmn.tanke756.top

cmd >/dev/null 2>&1
来源：http://fqv.zhongyouzk.top

[R42] 输入重定向
来源：http://alp.0kj1m.cn

wc -l < a.txt
来源：http://jwk.jinghuilouyu.cn

[R43] 按名字查找文件
来源：http://glj.chenjidiqi.icu

find . -name "*.log" -type f
来源：http://cyz.ivvv.top

[R44] 按修改时间查找
来源：http://zbm.chenjidiqi.icu

find . -mtime -7 -type f
来源：http://res.fengsongda.top

[R45] 批量删除
来源：http://lbo.aibaodan.cn

find . -name "*.tmp" -delete
来源：http://abl.fengsongda.top

[R46] 递归替换文件内容
来源：http://wrc.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://npe.quarkkingdee.top

[R47] sed 单行替换
来源：http://bmm.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://xfk.birdmap.top

[R48] awk 取指定列
来源：http://apj.hnqzz.top

awk '{print $1, $3}' a.txt
来源：http://kca.yongpay.top

[R49] awk 带条件
来源：http://erq.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lnf.cucudq.cn

[R50] awk 求和
来源：http://zoa.jinyuanbaomall.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mtm.gaohongyu789.top

[R51] 排序去重取前几
来源：http://fhc.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gra.mhx1999.top

[R52] 统计行数
来源：http://kwu.gaohongyu789.top

wc -l a.txt
来源：http://avd.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://twx.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zer.zhixingplan.top

[R54] 比较两个文件
来源：http://cvr.vehdjk.com

diff a.txt b.txt
来源：http://wdq.yuxming.cn

[R55] 压缩与解压
来源：http://iqp.iojbl.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xek.ydjk.org.cn

[R56] 远程拷贝
来源：http://iax.hysaishi.cn

scp file user@host:/path/
来源：http://rsn.yj20258.top

[R57] 远程执行命令
来源：http://fka.daria6918.cn

ssh user@host 'uptime'
来源：http://rcj.havefunace.top

[R58] 下载文件
来源：http://pxe.ydzc1.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nzl.jinqigufen.top

[R59] 发 POST JSON
来源：http://tej.hongshengwenyu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://toe.zhengqikj.top

[R60] 只看 HTTP 状态码
来源：http://skr.jyoumei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pyd.wangshuangyany.cn

[R61] 磁盘占用
来源：http://ion.yvedp.cn

df -h;  du -sh *
来源：http://rux.bbcook.cn

[R62] 找最占空间的文件
来源：http://mxb.snrcjt.cn

du -ah . | sort -rh | head -10
来源：http://bag.xinyue.icu

[R63] 内存与进程
来源：http://gyy.yonumen.top

free -h;  ps aux | grep nginx
来源：http://rsy.yj20258.top

[R64] 结束进程
来源：http://gmu.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://erl.sxryk.cn

[R65] 查看端口占用
来源：http://twc.nanxuanxn.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hok.bjfxy.top

[R66] 定时任务
来源：http://awk.mhx1999.top

crontab -e;  crontab -l
来源：http://sru.9152youxi.cn

[R67] 生成随机十六进制串
来源：http://dps.ydzc1.top

openssl rand -hex 16
来源：http://ogj.ppjwa.cn

[R68] 计算文件校验值
来源：http://zfl.quarkkingdee.top

sha256sum a.txt;  md5sum a.txt
来源：http://rjq.dianchejie.cn

[R69] 生成随机密码
来源：http://svr.xylfe.cn

head -c 16 /dev/urandom | base64
来源：http://nhc.bjfxy.top

[R70] 时间戳与互转
来源：http://uzb.hnqzz.top

date +%s;  date -d @1700000000
来源：http://tph.xingfuxueyuan.xyz

[R71] 日期格式化
来源：http://ept.ybcxt.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tko.svipenyu.cn

[R72] 等待端口就绪
来源：http://qvz.sxryk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dot.aibaodan.cn

[R73] 分割大日志
来源：http://cxt.zhongyouzk.top

split -l 1000 big.log part_
来源：http://wem.dashuyun.cn

[R74] 批量重命名
来源：http://agp.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hwq.guowangkeji.top

[R75] 导出环境变量
来源：http://rug.zycfv.cn

export PATH="$HOME/bin:$PATH"
来源：http://rre.yvedp.cn

[R76] 使用临时文件
来源：http://qjg.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mpq.pycfn.com

[R77] 读取用户输入
来源：http://sfe.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://uqh.nanxuanxn.top

[R78] 交互式菜单
来源：http://ebq.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://hsb.gaohongyu789.top

[R79] 解析命令行选项
来源：http://kzm.jinqigufen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gfq.shangyingyoupin.top

[R80] 查看脚本执行耗时
来源：http://aqv.cqqwz.cn

time ./run.sh
来源：http://ehm.hammf.cn

================================================================================
来源：http://pio.iojbl.cn

S. C / C++ 专题
来源：http://cmi.sysykeji.top

================================================================================
来源：http://dmt.sjlbkw.cn

[S01] C：Hello World
来源：http://fmu.pengpengdd.cyou

#include <stdio.h>
来源：http://icz.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dvy.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://poy.mhx1999.top

int a = 10; printf("%d\n", a);
来源：http://avh.zhengqikj.top

[S03] C：读入整数
来源：http://pch.ybcxt.top

int x; scanf("%d", &x);
来源：http://tin.mhx1999.top

[S04] C：字符串复制
来源：http://bwq.ybcxt.top

char dst[32]; strcpy(dst, "hi");
来源：http://mvg.jqgfzy.top

[S05] C：字符串长度
来源：http://vqq.hysaishi.cn

strlen(s)
来源：http://ilo.sweek.top

[S06] C：字符串比较
来源：http://knq.quarkkingdee.top

strcmp(a, b) == 0
来源：http://hzs.xingfuxueyuan.xyz

[S07] C：数组遍历求和
来源：http://eon.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://snn.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://slz.meibo888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wag.bbcook.cn

[S09] C：结构体定义与初始化
来源：http://tdi.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xqo.hnqzz.top

[S10] C：指针与解引用
来源：http://qau.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://xfu.yvedp.cn

[S11] C：逐行读文件
来源：http://ztr.tarul.cn

FILE *f = fopen("a.txt", "r");
来源：http://qpm.ydzc1.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dcn.sufxvd.cn

fclose(f);
来源：http://siv.yvedp.cn

[S12] C：写文件
来源：http://ldi.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nel.snrcjt.cn

[S13] C：宏定义
来源：http://jvr.zhengqikj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wqx.cqqwz.cn

[S14] C：枚举
来源：http://mjd.nanxuanxn.top

enum Color { RED, GREEN, BLUE };
来源：http://asw.c1oappe.top

[S15] C：类型转换
来源：http://pwu.pycfn.com

(double) a / b
来源：http://jqj.yj202588.top

[S16] C：位操作置位
来源：http://ala.tanke756.top

x |= (1 << 3);
来源：http://llx.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://qud.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://alx.zhoulong.xyz

[S18] C：命令行参数
来源：http://uqd.ywan-chungtsiang.top

int main(int argc, char **argv)
来源：http://utt.mhx1999.top

[S19] C：快速排序
来源：http://uis.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://eat.jinqigfzy.top

[S20] C：二分查找
来源：http://jdh.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qrt.xziqi.cn

[S21] C：字符类别判断
来源：http://utq.hammf.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cvz.wangdashe.top

[S22] C：字符串转数字
来源：http://igv.yj20258888.top

atoi("42");  strtod("3.14", NULL);
来源：http://fhd.svipenyu.cn

[S23] C：随机数
来源：http://qom.yonumen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://tde.tanke756.top

[S24] C：获取本地时间
来源：http://eix.aizwys.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hyn.haohaochexian.top

[S25] C：内存拷贝
来源：http://cez.birdmap.top

memcpy(dst, src, n);
来源：http://yfi.hcnkem.com

[S26] C：内存清零
来源：http://uyw.fktsv.cn

memset(a, 0, sizeof a);
来源：http://qkb.zhiwuduotai.top

[S27] C：定义常量
来源：http://dzx.andypj.xyz

const double PI = 3.14159;
来源：http://ewa.tanke756.top

[S28] C：静态变量
来源：http://xdl.bjfxy.top

static int counter = 0;
来源：http://jsm.mhx1999.top

[S29] C：变参函数
来源：http://whz.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://trz.cdnleiting.top

[S30] C：头文件保护
来源：http://rpu.nanxuanxn.top

#ifndef X_H
来源：http://mme.uphjek.com

#define X_H
来源：http://fqr.jqgufenzy.top

#endif
来源：http://vwm.gzhubu.top

[S31] C++：Hello World
来源：http://uch.316326.xyz

#include <iostream>
来源：http://gff.gaohongyu789.top

int main() { std::cout << "Hello\n"; }
来源：http://qbo.ydjk.org.cn

[S32] C++：字符串
来源：http://rne.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://iuw.haohaochexian.top

[S33] C++：vector 增删
来源：http://wyt.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hap.shangyingyoupin.top

[S34] C++：遍历 vector
来源：http://tyv.hnqzz.top

for (auto &x : v) { std::cout << x; }
来源：http://xje.daxiang520.top

[S35] C++：map
来源：http://gca.shuidangran.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lsl.tian-w.cn

[S36] C++：unordered_map
来源：http://jni.bjfxy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qtb.gogol.net.cn

[S37] C++：set
来源：http://tgc.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qja.xinyue.icu

[S38] C++：排序
来源：http://smx.jinyuanbaomall.cn

std::sort(v.begin(), v.end());
来源：http://zsp.tanke756.top

[S39] C++：自定义比较器排序
来源：http://sgw.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wfy.wangdashe.top

[S40] C++：查找元素
来源：http://ioq.pycfn.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ivd.hesvh.cn

[S41] C++：类与构造函数
来源：http://wsf.tianlin.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yvo.bjfxy.top

[S42] C++：继承与虚函数
来源：http://lws.hysaishi.cn

class B : public Base { public: void f() override {} };
来源：http://bbi.jianghu66.top

[S43] C++：智能指针
来源：http://weo.hongshengwenyu.top

auto p = std::make_unique<int>(5);
来源：http://lki.wangshuangyany.cn

[S44] C++：引用传参
来源：http://uou.uphjek.com

void inc(int &x) { ++x; }
来源：http://yth.hnxiangtu.top

[S45] C++：lambda
来源：http://wvv.jlsjyb.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qvr.uphjek.com

[S46] C++：函数模板
来源：http://zts.vehdjk.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bek.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://yid.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pym.gogol.net.cn

[S48] C++：逐行读文件
来源：http://iwu.chenlongwang.top

std::ifstream in("a.txt");  std::string line;
来源：http://xkh.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://lko.quarkkingdee.top

[S49] C++：写文件
来源：http://jiv.shangyingyoupin.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hsy.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://abk.zycfv.cn


<!-- 参考信息 -->