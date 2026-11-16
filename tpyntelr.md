代发 wailian999

[Q80] 字符串截取
来源：http://agm.sweek.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kkk.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://jpr.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lap.shuidangran.top

[Q82] 字符长度与字节长度
来源：http://nlv.jinqigufen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qzf.redwolf501.top

[Q83] 大小写转换
来源：http://uuj.zhiwuduotai.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ekb.zdbjq.cn

[Q84] 去除首尾空格
来源：http://smd.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://kja.aibaodan.cn

[Q85] 数值取整
来源：http://srg.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xfs.aizwys.cn

[Q86] 读取 JSON 字段
来源：http://vox.sufxvd.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ojq.shuidangran.top

[Q87] JSON 字段做条件
来源：http://usn.gotoacloud.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yhw.ppjwa.cn

[Q88] 行转列（条件聚合）
来源：http://asg.hywenlv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lml.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://erl.jlsjyb.cn

[Q89] 判断表是否存在
来源：http://syl.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zmm.yangfankeji.com

[Q90] 生成序号列
来源：http://qwi.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tgy.chenjidiqi.icu

================================================================================
来源：http://swh.jinghuilouyu.cn

R. Bash 专题
来源：http://rbb.zhiwuduotai.top

================================================================================
来源：http://oly.jiagoushi.top

[R01] shebang 与严格模式
来源：http://ike.52xcode.cn

#!/usr/bin/env bash
来源：http://wiy.tian-w.cn

set -euo pipefail
来源：http://gzs.fzhhl.top

[R02] 变量赋值与使用
来源：http://pdf.smart0.xyz

name="Tom"; echo "$name"
来源：http://pqb.shuidangran.top

[R03] 只读变量
来源：http://pmx.sufxvd.cn

readonly PI=3.14
来源：http://kju.zycfv.cn

[R04] 位置参数
来源：http://zoh.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xyq.shuidangran.top

[R05] 参数默认值
来源：http://okj.ydzc1.top

name="${1:-default}"
来源：http://gyv.yj20258888.top

[R06] 判断命令是否存在
来源：http://qza.shuidangran.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eee.ybcxt.top

[R07] if 判断文件
来源：http://htu.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vfi.bjfxy.top

[R08] 数值比较
来源：http://gct.yuxming.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lih.xingfuxueyuan.xyz

[R09] 字符串比较
来源：http://dyh.feifeiyinyue.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xch.zhoulong.xyz

[R10] 正则匹配
来源：http://jui.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ear.zycfv.cn

[R11] case 多分支
来源：http://cpk.nanxuanxn.top

case "$1" in
来源：http://oqr.fktsv.cn

start) echo "启动" ;;
来源：http://fta.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://ziz.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://jgl.dashuyun.cn

esac
来源：http://qas.vqdsnc.cn

[R12] for 遍历文件
来源：http://kfw.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://tjv.cucudq.cn

[R13] for 计数循环
来源：http://lko.yueranfly.top

for i in {1..10}; do echo "$i"; done
来源：http://fwe.yueranfly.top

[R14] C 风格 for
来源：http://cmu.havefunace.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gtd.hywenlv.cn

[R15] while 逐行读文件
来源：http://rwk.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wos.ydjk.org.cn

[R16] until 等待条件
来源：http://vkp.ydjk.org.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gnt.tian-w.cn

[R17] 数组定义与取值
来源：http://ajc.birdmap.top

arr=(a b c); echo "${arr[0]}"
来源：http://eeu.fzhhl.top

[R18] 遍历数组
来源：http://clf.nanxuanxn.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://arc.jinqigufen.top

[R19] 数组长度
来源：http://cqn.yonumen.top

echo "${#arr[@]}"
来源：http://wya.svipenyu.cn

[R20] 关联数组（字典）
来源：http://mhb.xylfe.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qeg.guowangkeji.top

[R21] 字符串长度
来源：http://aru.zhoulong.xyz

echo "${#s}"
来源：http://wxo.nanxinkj.top

[R22] 截取子串
来源：http://kxu.yj20258888.top

echo "${s:0:5}"
来源：http://ump.0kj1m.cn

[R23] 字符串替换
来源：http://exr.yfazqb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rmm.guannengcc.top

[R24] 大小写转换
来源：http://vkh.tanke756.top

echo "${s^^}"; echo "${s,,}"
来源：http://qdi.birdmap.top

[R25] 去后缀 / 去前缀
来源：http://kpt.yanxiufei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://piq.gotoacloud.top

[R26] 命令替换
来源：http://zma.pengpengdd.cyou

now=$(date +%F); echo "$now"
来源：http://ipw.nwbrower.top

[R27] 算术展开
来源：http://xzh.xuanzx.com

echo $((1 + 2 * 3))
来源：http://rie.zycfv.cn

[R28] 浮点运算
来源：http://otr.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://lpf.jinghuilouyu.cn

[R29] 定义函数
来源：http://mry.jqgfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bcr.gaohongyu789.top

[R30] 函数返回状态码
来源：http://vks.tarul.cn

f() { return 0; }; f || echo "失败了"
来源：http://jml.chenlongwang.top

[R31] 局部变量
来源：http://nye.dashuyun.cn

f() { local x=1; echo "$x"; }
来源：http://mmj.cdnleiting.top

[R32] 参数个数校验
来源：http://swx.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kkf.yj20258.top

[R33] 捕获错误并提示行号
来源：http://vlx.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oxj.gaohongyu789.top

[R34] 退出时清理
来源：http://elj.snrcjt.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rfx.cucudq.cn

[R35] 后台执行并等待
来源：http://bcs.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://uwh.zhengqikj.top

[R36] 并发执行多个任务
来源：http://kzi.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://trm.vqdsnc.cn

[R37] 把输出赋给变量
来源：http://vlu.hnqzz.top

files=$(ls -1)
来源：http://cal.ydjk.org.cn

[R38] 管道串联
来源：http://igj.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://eoj.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://lia.sysykeji.top

cmd > out.log 2>&1
来源：http://wep.gzhubu.top

[R40] 追加写日志
来源：http://kzd.fanxiaobao.xyz

echo "log" >> out.log
来源：http://gds.svipenyu.cn

[R41] 丢弃输出
来源：http://ddu.daria6918.cn

cmd >/dev/null 2>&1
来源：http://djq.sufxvd.cn

[R42] 输入重定向
来源：http://aqx.shanyushiyangtech.top

wc -l < a.txt
来源：http://kao.aizwys.cn

[R43] 按名字查找文件
来源：http://orw.epnwcf.com

find . -name "*.log" -type f
来源：http://cen.sjlbkw.cn

[R44] 按修改时间查找
来源：http://uqc.zhoulong.xyz

find . -mtime -7 -type f
来源：http://edz.jqgufenzy.top

[R45] 批量删除
来源：http://wvi.zhaomingkeji.xyz

find . -name "*.tmp" -delete
来源：http://apt.yuanzhike.top

[R46] 递归替换文件内容
来源：http://kbz.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fhn.dashuyun.cn

[R47] sed 单行替换
来源：http://xlx.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://ocn.52xcode.cn

[R48] awk 取指定列
来源：http://eii.meibo888.top

awk '{print $1, $3}' a.txt
来源：http://lqh.shangyingyoupin.top

[R49] awk 带条件
来源：http://vqs.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gkx.zdbjq.cn

[R50] awk 求和
来源：http://roh.ehwqpu.com

awk '{s += $2} END {print s}' a.txt
来源：http://jdi.cucudq.cn

[R51] 排序去重取前几
来源：http://uiy.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rpw.jyoumei.cn

[R52] 统计行数
来源：http://fwe.uphjek.com

wc -l a.txt
来源：http://aaa.cashguo.top

[R53] 查看文件头与实时尾
来源：http://wky.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gei.shangyingyoupin.top

[R54] 比较两个文件
来源：http://kdx.cdnleiting.top

diff a.txt b.txt
来源：http://mlw.hongshengwenyu.top

[R55] 压缩与解压
来源：http://ysj.shanyushiyangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qow.jiagoushi.top

[R56] 远程拷贝
来源：http://bdh.tanke756.top

scp file user@host:/path/
来源：http://lub.zhixingplan.top

[R57] 远程执行命令
来源：http://qyd.yanxiufei.cn

ssh user@host 'uptime'
来源：http://pwh.jlsjyb.cn

[R58] 下载文件
来源：http://nqg.fengsongda.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pny.vqdsnc.cn

[R59] 发 POST JSON
来源：http://igc.tian-w.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vya.shangyingyoupin.top

[R60] 只看 HTTP 状态码
来源：http://opy.epnwcf.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uog.wangshuangyany.cn

[R61] 磁盘占用
来源：http://hbv.fengsongda.top

df -h;  du -sh *
来源：http://hdi.aizwys.cn

[R62] 找最占空间的文件
来源：http://lkf.haohaochexian.top

du -ah . | sort -rh | head -10
来源：http://yjv.jianghu66.top

[R63] 内存与进程
来源：http://rmx.zhijiandao.cn

free -h;  ps aux | grep nginx
来源：http://axo.jqgufenzy.top

[R64] 结束进程
来源：http://xsc.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://otg.hesvh.cn

[R65] 查看端口占用
来源：http://cry.gotoacloud.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://irw.nanxuanxn.top

[R66] 定时任务
来源：http://uhd.daxiang520.top

crontab -e;  crontab -l
来源：http://qsm.aizwys.cn

[R67] 生成随机十六进制串
来源：http://nuu.jqgfzy.top

openssl rand -hex 16
来源：http://hlw.chenzaomai.com

[R68] 计算文件校验值
来源：http://dfl.epnwcf.com

sha256sum a.txt;  md5sum a.txt
来源：http://nlw.dianchejie.cn

[R69] 生成随机密码
来源：http://vbo.yj20258888.top

head -c 16 /dev/urandom | base64
来源：http://rzn.zhiwuduotai.top

[R70] 时间戳与互转
来源：http://ncr.ywan-chungtsiang.top

date +%s;  date -d @1700000000
来源：http://tfn.ehwqpu.com

[R71] 日期格式化
来源：http://dkp.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vok.cucudq.cn

[R72] 等待端口就绪
来源：http://kff.iojbl.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yfr.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://uxb.xziqi.cn

split -l 1000 big.log part_
来源：http://ioy.hfpthk.cn

[R74] 批量重命名
来源：http://hor.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rmn.nwbrower.top

[R75] 导出环境变量
来源：http://mcr.chenzaomai.com

export PATH="$HOME/bin:$PATH"
来源：http://xwe.iojbl.cn

[R76] 使用临时文件
来源：http://zjh.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hll.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://lya.cashguo.top

read -rp "请输入: " ans
来源：http://eig.hongshengwenyu.top

[R78] 交互式菜单
来源：http://mfh.ybcxt.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ils.jinqigfzy.top

[R79] 解析命令行选项
来源：http://agf.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rym.fehbvm.com

[R80] 查看脚本执行耗时
来源：http://thm.ydjk.org.cn

time ./run.sh
来源：http://est.jinghuilouyu.cn

================================================================================
来源：http://bpd.redwolf501.top

S. C / C++ 专题
来源：http://wxv.zhongyouzk.top

================================================================================
来源：http://mbn.yanxiufei.cn

[S01] C：Hello World
来源：http://zgl.xuetiantiany.cn

#include <stdio.h>
来源：http://eeo.hnqzz.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vfb.daxiang520.top

[S02] C：变量与格式化输出
来源：http://iuw.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://jon.zycfv.cn

[S03] C：读入整数
来源：http://lbb.shanyushiyangtech.top

int x; scanf("%d", &x);
来源：http://eqk.jinqigfzy.top

[S04] C：字符串复制
来源：http://occ.hnqzz.top

char dst[32]; strcpy(dst, "hi");
来源：http://cbq.vqdsnc.cn

[S05] C：字符串长度
来源：http://gul.fzhhl.top

strlen(s)
来源：http://jmn.ehwqpu.com

[S06] C：字符串比较
来源：http://ywn.shzxlz.cn

strcmp(a, b) == 0
来源：http://usf.tanke756.top

[S07] C：数组遍历求和
来源：http://wxf.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zpn.xuanzx.com

[S08] C：动态内存分配与释放
来源：http://ilv.yuxming.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xxx.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://sbx.sjlbkw.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fbu.cashguo.top

[S10] C：指针与解引用
来源：http://mau.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://sxr.shuidangran.top

[S11] C：逐行读文件
来源：http://pph.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://mvv.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rcu.hysaishi.cn

fclose(f);
来源：http://tfy.yonumen.top

[S12] C：写文件
来源：http://ajv.hnqzz.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xaw.cqqwz.cn

[S13] C：宏定义
来源：http://jrn.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xzr.gogol.net.cn

[S14] C：枚举
来源：http://czx.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://qix.tanke756.top

[S15] C：类型转换
来源：http://ayq.ywan-chungtsiang.top

(double) a / b
来源：http://cpf.bbcook.cn

[S16] C：位操作置位
来源：http://tfb.9152youxi.cn

x |= (1 << 3);
来源：http://wig.vqdsnc.cn

[S17] C：安全拼接字符串
来源：http://nfp.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zer.0kj1m.cn

[S18] C：命令行参数
来源：http://xti.yueranfly.top

int main(int argc, char **argv)
来源：http://zpr.meibo888.top

[S19] C：快速排序
来源：http://nkg.zhoulong.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://stv.zdbjq.cn

[S20] C：二分查找
来源：http://rru.zhengqikj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://olt.birdmap.top

[S21] C：字符类别判断
来源：http://ntr.fengsongda.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nnm.yanxiufei.cn

[S22] C：字符串转数字
来源：http://usj.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://daf.fanxiaobao.xyz

[S23] C：随机数
来源：http://xfw.sysykeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gim.wangdashe.top

[S24] C：获取本地时间
来源：http://jml.fanxiaobao.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ulp.uphjek.com

[S25] C：内存拷贝
来源：http://ewi.xuanzx.com

memcpy(dst, src, n);
来源：http://hcv.aizwys.cn

[S26] C：内存清零
来源：http://xco.ctjpmb.com

memset(a, 0, sizeof a);
来源：http://eka.ctjpmb.com

[S27] C：定义常量
来源：http://fck.cqqwz.cn

const double PI = 3.14159;
来源：http://xzm.jyoumei.cn

[S28] C：静态变量
来源：http://rtk.shuidangran.top

static int counter = 0;
来源：http://hwm.daria6918.cn

[S29] C：变参函数
来源：http://hbr.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://veu.xuanzx.com

[S30] C：头文件保护
来源：http://xjj.zhijiandao.cn

#ifndef X_H
来源：http://qzu.dianchejie.cn

#define X_H
来源：http://erj.ydjk.org.cn

#endif
来源：http://hvs.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://xbt.cucudq.cn

#include <iostream>
来源：http://szx.zhengqikj.top

int main() { std::cout << "Hello\n"; }
来源：http://wue.xziqi.cn

[S32] C++：字符串
来源：http://wsu.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://cpi.shuidangran.top

[S33] C++：vector 增删
来源：http://xuq.jiagoushi.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://typ.fengsongda.top

[S34] C++：遍历 vector
来源：http://fwk.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://zsf.sufxvd.cn

[S35] C++：map
来源：http://vdu.tianlin.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pgn.cashguo.top

[S36] C++：unordered_map
来源：http://bon.jinghuilouyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gic.sjlbkw.cn

[S37] C++：set
来源：http://nvj.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vux.snrcjt.cn

[S38] C++：排序
来源：http://pfd.wangshuangyany.cn

std::sort(v.begin(), v.end());
来源：http://gto.wangdashe.top

[S39] C++：自定义比较器排序
来源：http://kdv.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hwb.yvedp.cn

[S40] C++：查找元素
来源：http://ewt.gotoacloud.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cte.andypj.xyz

[S41] C++：类与构造函数
来源：http://lrb.haohaochexian.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ube.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://aow.fanxiaobao.xyz

class B : public Base { public: void f() override {} };
来源：http://kkt.yfazqb.com

[S43] C++：智能指针
来源：http://vdz.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://imw.tanke756.top

[S44] C++：引用传参
来源：http://ojj.hongshengwenyu.top

void inc(int &x) { ++x; }
来源：http://yok.bjfxy.top

[S45] C++：lambda
来源：http://aad.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://ehb.mhx1999.top

[S46] C++：函数模板
来源：http://mvc.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pji.jqgufenzy.top

[S47] C++：结构化绑定遍历
来源：http://joz.gaohongyu789.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qjx.iojbl.cn

[S48] C++：逐行读文件
来源：http://tmn.iojbl.cn

std::ifstream in("a.txt");  std::string line;
来源：http://aaa.chenjidiqi.icu

while (std::getline(in, line)) { }
来源：http://imr.0kj1m.cn

[S49] C++：写文件
来源：http://zkr.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.gzhubu.top

[S50] C++：格式化数字
来源：http://rag.yj202588.top


<!-- 参考信息 -->