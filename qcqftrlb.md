代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wbh.hesvh.cn

[Q75] 日期格式化
来源：http://akq.daxiang520.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gie.chenjidiqi.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oeh.hysaishi.cn

[Q76] 按天统计
来源：http://ctk.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tje.vehdjk.com

[Q77] 时间加减
来源：http://eng.smart0.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pma.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://sgq.yuxming.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://exu.zycfv.cn

[Q79] 字符串拼接
来源：http://whu.ydzc1.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mob.ehwqpu.com

[Q80] 字符串截取
来源：http://nlz.yfazqb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rxt.yonumen.top

[Q81] 字符串替换
来源：http://eil.bjfxy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kik.hnqzz.top

[Q82] 字符长度与字节长度
来源：http://nqn.jlsjyb.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://peq.zhaomingkeji.xyz

[Q83] 大小写转换
来源：http://sjp.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kzq.zhongyouzk.top

[Q84] 去除首尾空格
来源：http://kwy.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://oow.hnqzz.top

[Q85] 数值取整
来源：http://swh.zhixingplan.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vii.jiagoushi.top

[Q86] 读取 JSON 字段
来源：http://squ.zhiwuduotai.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tlv.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://kkp.cheryme.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ylc.sweek.top

[Q88] 行转列（条件聚合）
来源：http://kcl.guannengcc.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sfx.cqqwz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pyy.shuidangran.top

[Q89] 判断表是否存在
来源：http://wye.zhaomingkeji.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iwq.yfazqb.com

[Q90] 生成序号列
来源：http://nfo.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://egk.meibo888.top

================================================================================
来源：http://sbs.sxryk.cn

R. Bash 专题
来源：http://zpi.yj20258.top

================================================================================
来源：http://vuk.tanke756.top

[R01] shebang 与严格模式
来源：http://tue.hywenlv.cn

#!/usr/bin/env bash
来源：http://mdx.xylfe.cn

set -euo pipefail
来源：http://ciu.zdqjudy.top

[R02] 变量赋值与使用
来源：http://bew.ctjpmb.com

name="Tom"; echo "$name"
来源：http://rtj.xinyue.icu

[R03] 只读变量
来源：http://gbi.chenjidiqi.icu

readonly PI=3.14
来源：http://gms.pycfn.com

[R04] 位置参数
来源：http://mrl.nanxuanxn.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ptr.yuxming.cn

[R05] 参数默认值
来源：http://vep.daxiang520.top

name="${1:-default}"
来源：http://mpk.yvedp.cn

[R06] 判断命令是否存在
来源：http://ndk.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ipy.yongpay.top

[R07] if 判断文件
来源：http://xev.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mcr.dashuyun.cn

[R08] 数值比较
来源：http://fbz.bbcook.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xju.ybcxt.top

[R09] 字符串比较
来源：http://wys.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xnc.zhixingplan.top

[R10] 正则匹配
来源：http://uvs.gogol.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qmd.ydzc1.top

[R11] case 多分支
来源：http://uel.tanke756.top

case "$1" in
来源：http://gdv.hongshengwenyu.top

start) echo "启动" ;;
来源：http://hpx.zdbjq.cn

stop)  echo "停止" ;;
来源：http://zdj.fanxiaobao.xyz

*)     echo "未知命令" ;;
来源：http://vwu.c1oappe.top

esac
来源：http://bry.yongpay.top

[R12] for 遍历文件
来源：http://iox.xylfe.cn

for f in *.txt; do echo "$f"; done
来源：http://vjp.dashuyun.cn

[R13] for 计数循环
来源：http://gmq.sysykeji.top

for i in {1..10}; do echo "$i"; done
来源：http://sry.jqgufenzy.top

[R14] C 风格 for
来源：http://ial.yuxming.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cak.nwbrower.top

[R15] while 逐行读文件
来源：http://sxb.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ckh.fktsv.cn

[R16] until 等待条件
来源：http://gvi.epnwcf.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://byz.yonumen.top

[R17] 数组定义与取值
来源：http://yup.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://zfu.dashuyun.cn

[R18] 遍历数组
来源：http://dxc.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jsp.yuanzhike.top

[R19] 数组长度
来源：http://ewu.hcnkem.com

echo "${#arr[@]}"
来源：http://rhu.wangshuangyany.cn

[R20] 关联数组（字典）
来源：http://emz.snrcjt.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bvh.hywenlv.cn

[R21] 字符串长度
来源：http://fvy.jinyuanbaomall.cn

echo "${#s}"
来源：http://wfw.chenjidiqi.icu

[R22] 截取子串
来源：http://cry.nwbrower.top

echo "${s:0:5}"
来源：http://kfv.gogol.net.cn

[R23] 字符串替换
来源：http://lku.pycfn.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bsh.ehwqpu.com

[R24] 大小写转换
来源：http://rtf.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://mkg.fanxiaobao.xyz

[R25] 去后缀 / 去前缀
来源：http://sht.hnxiangtu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tca.chenjidiqi.icu

[R26] 命令替换
来源：http://wyg.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://sak.zhongyouzk.top

[R27] 算术展开
来源：http://hij.cucudq.cn

echo $((1 + 2 * 3))
来源：http://rhy.uphjek.com

[R28] 浮点运算
来源：http://yee.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://had.9152youxi.cn

[R29] 定义函数
来源：http://srq.zdqjudy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tom.svipenyu.cn

[R30] 函数返回状态码
来源：http://ykh.52xcode.cn

f() { return 0; }; f || echo "失败了"
来源：http://mnk.fanxiaobao.xyz

[R31] 局部变量
来源：http://qxe.zhengqikj.top

f() { local x=1; echo "$x"; }
来源：http://reh.zhixingplan.top

[R32] 参数个数校验
来源：http://fvd.hesvh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vaw.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://aij.yangfankeji.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ivp.tian-w.cn

[R34] 退出时清理
来源：http://mxs.fzhhl.top

trap 'rm -f "$tmp"' EXIT
来源：http://tnk.fzhhl.top

[R35] 后台执行并等待
来源：http://mxm.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://pfa.redwolf501.top

[R36] 并发执行多个任务
来源：http://ima.yj202588.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ups.jyoumei.cn

[R37] 把输出赋给变量
来源：http://wxp.tanke756.top

files=$(ls -1)
来源：http://bgc.chenlongwang.top

[R38] 管道串联
来源：http://faw.cheryme.top

cat a.txt | grep -i error | wc -l
来源：http://zob.hcnkem.com

[R39] 重定向标准输出与错误
来源：http://rme.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://sjh.hywenlv.cn

[R40] 追加写日志
来源：http://dla.hongshengwenyu.top

echo "log" >> out.log
来源：http://rsz.hywenlv.cn

[R41] 丢弃输出
来源：http://bug.daxiang520.top

cmd >/dev/null 2>&1
来源：http://djp.aizwys.cn

[R42] 输入重定向
来源：http://xfz.shzxlz.cn

wc -l < a.txt
来源：http://xvx.jiagoushi.top

[R43] 按名字查找文件
来源：http://yqe.iojbl.cn

find . -name "*.log" -type f
来源：http://wax.zhijiandao.cn

[R44] 按修改时间查找
来源：http://els.ydzc1.top

find . -mtime -7 -type f
来源：http://nop.ehwqpu.com

[R45] 批量删除
来源：http://ehw.fzhhl.top

find . -name "*.tmp" -delete
来源：http://sfe.xuetiantiany.cn

[R46] 递归替换文件内容
来源：http://spb.birdmap.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yaq.chenzaomai.com

[R47] sed 单行替换
来源：http://xun.wangdashe.top

sed -i 's/foo/bar/g' a.txt
来源：http://uje.jyoumei.cn

[R48] awk 取指定列
来源：http://tlw.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://xly.zhoulong.xyz

[R49] awk 带条件
来源：http://jwo.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vwc.vehdjk.com

[R50] awk 求和
来源：http://qbf.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://hqv.zhengqikj.top

[R51] 排序去重取前几
来源：http://lnk.haohaochexian.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lho.yueranfly.top

[R52] 统计行数
来源：http://cqg.iojbl.cn

wc -l a.txt
来源：http://bch.andypj.xyz

[R53] 查看文件头与实时尾
来源：http://opl.bbcook.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lwp.vqdsnc.cn

[R54] 比较两个文件
来源：http://cvb.zdbjq.cn

diff a.txt b.txt
来源：http://tqe.yj20258888.top

[R55] 压缩与解压
来源：http://yuz.hammf.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ykh.ppjwa.cn

[R56] 远程拷贝
来源：http://xut.hammf.cn

scp file user@host:/path/
来源：http://wde.aibaodan.cn

[R57] 远程执行命令
来源：http://amd.zdqjudy.top

ssh user@host 'uptime'
来源：http://bsx.fktsv.cn

[R58] 下载文件
来源：http://owa.gotoacloud.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mpf.shuidangran.top

[R59] 发 POST JSON
来源：http://lkh.dianchejie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ewy.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://erg.tianlin.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pyt.xylfe.cn

[R61] 磁盘占用
来源：http://oqi.c1oappe.top

df -h;  du -sh *
来源：http://nqk.yongpay.top

[R62] 找最占空间的文件
来源：http://kri.316326.xyz

du -ah . | sort -rh | head -10
来源：http://zon.feifeiyinyue.top

[R63] 内存与进程
来源：http://dbf.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://dud.ppjwa.cn

[R64] 结束进程
来源：http://tdu.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://lln.shzxlz.cn

[R65] 查看端口占用
来源：http://xll.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dgj.yongpay.top

[R66] 定时任务
来源：http://tsp.yongpay.top

crontab -e;  crontab -l
来源：http://eov.fehbvm.com

[R67] 生成随机十六进制串
来源：http://qoh.vehdjk.com

openssl rand -hex 16
来源：http://ycq.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://gmf.shuidangran.top

sha256sum a.txt;  md5sum a.txt
来源：http://lqr.52xcode.cn

[R69] 生成随机密码
来源：http://til.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://srs.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://suu.wangdashe.top

date +%s;  date -d @1700000000
来源：http://dwd.jinqigufen.top

[R71] 日期格式化
来源：http://vzq.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vkl.cucudq.cn

[R72] 等待端口就绪
来源：http://uza.tian-w.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hzc.316326.xyz

[R73] 分割大日志
来源：http://cym.tanke756.top

split -l 1000 big.log part_
来源：http://bdw.0kj1m.cn

[R74] 批量重命名
来源：http://wyt.ehwqpu.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tvu.yonumen.top

[R75] 导出环境变量
来源：http://pik.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://zdo.jinqigfzy.top

[R76] 使用临时文件
来源：http://fvs.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yth.hesvh.cn

[R77] 读取用户输入
来源：http://hoi.aizwys.cn

read -rp "请输入: " ans
来源：http://stq.dashuyun.cn

[R78] 交互式菜单
来源：http://qfa.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hjq.xinyue.icu

[R79] 解析命令行选项
来源：http://oml.0kj1m.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://umm.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://qlh.pycfn.com

time ./run.sh
来源：http://coy.daria6918.cn

================================================================================
来源：http://mcf.hesvh.cn

S. C / C++ 专题
来源：http://vwc.hongshengwenyu.top

================================================================================
来源：http://nyg.yangfankeji.com

[S01] C：Hello World
来源：http://qzi.cheryme.top

#include <stdio.h>
来源：http://hbr.zdqjudy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://oht.yonumen.top

[S02] C：变量与格式化输出
来源：http://ppn.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://tln.gotoacloud.top

[S03] C：读入整数
来源：http://qoz.cheryme.top

int x; scanf("%d", &x);
来源：http://zdd.zhaomingkeji.xyz

[S04] C：字符串复制
来源：http://xec.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://yam.nanxuanxn.top

[S05] C：字符串长度
来源：http://vqp.0kj1m.cn

strlen(s)
来源：http://omu.jinqigfzy.top

[S06] C：字符串比较
来源：http://qzd.yj20258.top

strcmp(a, b) == 0
来源：http://mwl.ivvv.top

[S07] C：数组遍历求和
来源：http://vtk.ywan-chungtsiang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jyq.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://ssu.fengsongda.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://txp.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://jtd.pycfn.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vve.tanke756.top

[S10] C：指针与解引用
来源：http://xmy.shanyushiyangtech.top

int *p = &a;  *p = 5;
来源：http://zri.bbcook.cn

[S11] C：逐行读文件
来源：http://mix.9152youxi.cn

FILE *f = fopen("a.txt", "r");
来源：http://hht.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gmq.yj20258888.top

fclose(f);
来源：http://gus.aizwys.cn

[S12] C：写文件
来源：http://xci.chenzaomai.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jpk.zycfv.cn

[S13] C：宏定义
来源：http://hix.fktsv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ijj.xylfe.cn

[S14] C：枚举
来源：http://itu.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://yrq.smart0.xyz

[S15] C：类型转换
来源：http://jtm.fehbvm.com

(double) a / b
来源：http://ieg.guowangkeji.top

[S16] C：位操作置位
来源：http://zbd.aibaodan.cn

x |= (1 << 3);
来源：http://zxa.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://cfz.zhengqikj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jwp.smart0.xyz

[S18] C：命令行参数
来源：http://bdd.hfpthk.cn

int main(int argc, char **argv)
来源：http://ndn.uphjek.com

[S19] C：快速排序
来源：http://gkl.yj20258.top

qsort(a, n, sizeof(int), cmp);
来源：http://qkc.shzxlz.cn

[S20] C：二分查找
来源：http://kfd.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ysb.dianchejie.cn

[S21] C：字符类别判断
来源：http://sdo.fengsongda.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eok.iojbl.cn

[S22] C：字符串转数字
来源：http://stc.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://icd.fanxiaobao.xyz

[S23] C：随机数
来源：http://wmu.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lwh.yj202588.top

[S24] C：获取本地时间
来源：http://tpe.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qpz.ydjk.org.cn

[S25] C：内存拷贝
来源：http://wfr.ybcxt.top

memcpy(dst, src, n);
来源：http://rxa.shuidangran.top

[S26] C：内存清零
来源：http://wgs.yj202588.top

memset(a, 0, sizeof a);
来源：http://oje.vehdjk.com

[S27] C：定义常量
来源：http://igd.snrcjt.cn

const double PI = 3.14159;
来源：http://hep.feifeiyinyue.top

[S28] C：静态变量
来源：http://utz.shzxlz.cn

static int counter = 0;
来源：http://ybq.daria6918.cn

[S29] C：变参函数
来源：http://ysf.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://znf.uphjek.com

[S30] C：头文件保护
来源：http://zrc.dashuyun.cn

#ifndef X_H
来源：http://eha.jyoumei.cn

#define X_H
来源：http://zrr.tian-w.cn

#endif
来源：http://spu.zhiwuduotai.top

[S31] C++：Hello World
来源：http://kzr.chenzaomai.com

#include <iostream>
来源：http://rgi.ydzc1.top

int main() { std::cout << "Hello\n"; }
来源：http://qfc.shanyushiyangtech.top

[S32] C++：字符串
来源：http://tpx.yanxiufei.cn

std::string s = "hi";  s += "!";
来源：http://drg.chenlongwang.top

[S33] C++：vector 增删
来源：http://psb.xuetiantiany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://waa.hysaishi.cn

[S34] C++：遍历 vector
来源：http://lso.fanxiaobao.xyz

for (auto &x : v) { std::cout << x; }
来源：http://gqu.jqgfzy.top

[S35] C++：map
来源：http://lgw.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sho.jqgufenzy.top

[S36] C++：unordered_map
来源：http://viz.shzxlz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ebm.yj20258.top

[S37] C++：set
来源：http://ljw.snrcjt.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://efd.yueranfly.top

[S38] C++：排序
来源：http://nhw.nanxuanxn.top

std::sort(v.begin(), v.end());
来源：http://hrs.aizwys.cn

[S39] C++：自定义比较器排序
来源：http://ios.jinyuanbaomall.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rhb.hongshengwenyu.top

[S40] C++：查找元素
来源：http://smf.zhijiandao.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jdt.hongshengwenyu.top

[S41] C++：类与构造函数
来源：http://swy.jinyuanbaomall.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gep.meibo888.top

[S42] C++：继承与虚函数
来源：http://bbo.wangdashe.top

class B : public Base { public: void f() override {} };
来源：http://cvl.fengsongda.top

[S43] C++：智能指针
来源：http://ksc.xingfuxueyuan.xyz

auto p = std::make_unique<int>(5);
来源：http://ptx.zhijiandao.cn

[S44] C++：引用传参
来源：http://ceo.jianghu66.top

void inc(int &x) { ++x; }
来源：http://xup.jqgufenzy.top


<!-- 参考信息 -->