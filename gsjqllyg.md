代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lcx.cqqwz.cn

[Q75] 日期格式化
来源：http://dea.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rne.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gnr.birdmap.top

[Q76] 按天统计
来源：http://zaa.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://epn.nanxinkj.top

[Q77] 时间加减
来源：http://eto.snrcjt.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qeu.aizwys.cn

[Q78] 当前时间
来源：http://mpi.snrcjt.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vrp.9152youxi.cn

[Q79] 字符串拼接
来源：http://qyi.yueranfly.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ozf.zhaomingkeji.xyz

[Q80] 字符串截取
来源：http://fft.hnqzz.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bud.chenjidiqi.icu

[Q81] 字符串替换
来源：http://ifz.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fyc.uphjek.com

[Q82] 字符长度与字节长度
来源：http://ver.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ddn.sufxvd.cn

[Q83] 大小写转换
来源：http://jzo.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fgh.uphjek.com

[Q84] 去除首尾空格
来源：http://niu.hnxiangtu.top

SELECT TRIM(name) FROM users;
来源：http://dvt.yangfankeji.com

[Q85] 数值取整
来源：http://qbp.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lwu.guowangkeji.top

[Q86] 读取 JSON 字段
来源：http://qmo.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://umj.zhixingplan.top

[Q87] JSON 字段做条件
来源：http://vfy.fktsv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kjz.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://nzz.9152youxi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://isk.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sze.sufxvd.cn

[Q89] 判断表是否存在
来源：http://rns.zhoulong.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oqz.hcnkem.com

[Q90] 生成序号列
来源：http://qgv.ppjwa.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oug.jiagoushi.top

================================================================================
来源：http://wpb.fktsv.cn

R. Bash 专题
来源：http://jgu.cucudq.cn

================================================================================
来源：http://dzy.tianlin.xyz

[R01] shebang 与严格模式
来源：http://cvh.zdbjq.cn

#!/usr/bin/env bash
来源：http://kha.9152youxi.cn

set -euo pipefail
来源：http://ofz.feifeiyinyue.top

[R02] 变量赋值与使用
来源：http://xim.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://gdq.pengpengdd.cyou

[R03] 只读变量
来源：http://asq.vehdjk.com

readonly PI=3.14
来源：http://xjy.yj20258.top

[R04] 位置参数
来源：http://vgv.jqgufenzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gyc.yfazqb.com

[R05] 参数默认值
来源：http://uts.316326.xyz

name="${1:-default}"
来源：http://ofz.cdnleiting.top

[R06] 判断命令是否存在
来源：http://ery.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nsc.daxiang520.top

[R07] if 判断文件
来源：http://upr.gaohongyu789.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lxa.hongshengwenyu.top

[R08] 数值比较
来源：http://exi.yuxming.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ubb.jinqigfzy.top

[R09] 字符串比较
来源：http://zvx.jyoumei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://knq.jinghuilouyu.cn

[R10] 正则匹配
来源：http://wtr.ppjwa.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://boy.jianghu66.top

[R11] case 多分支
来源：http://zpz.quarkkingdee.top

case "$1" in
来源：http://ogv.hammf.cn

start) echo "启动" ;;
来源：http://oct.gzhubu.top

stop)  echo "停止" ;;
来源：http://rza.snrcjt.cn

*)     echo "未知命令" ;;
来源：http://bhr.sxryk.cn

esac
来源：http://kso.cdnleiting.top

[R12] for 遍历文件
来源：http://whb.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://szo.jinghuilouyu.cn

[R13] for 计数循环
来源：http://ucj.yuanzhike.top

for i in {1..10}; do echo "$i"; done
来源：http://lam.ehwqpu.com

[R14] C 风格 for
来源：http://yyu.havefunace.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dpq.aizwys.cn

[R15] while 逐行读文件
来源：http://mlc.zycfv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pbx.yfazqb.com

[R16] until 等待条件
来源：http://gqm.shanyushiyangtech.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qtb.chenlongwang.top

[R17] 数组定义与取值
来源：http://gnz.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gil.andypj.xyz

[R18] 遍历数组
来源：http://ajv.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rcr.jqgufenzy.top

[R19] 数组长度
来源：http://jpd.xuetiantiany.cn

echo "${#arr[@]}"
来源：http://ljf.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://tvu.pengpengdd.cyou

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tow.hnqzz.top

[R21] 字符串长度
来源：http://lgp.xziqi.cn

echo "${#s}"
来源：http://uhy.cqqwz.cn

[R22] 截取子串
来源：http://auz.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://gdy.yonumen.top

[R23] 字符串替换
来源：http://wse.xziqi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zcu.ppjwa.cn

[R24] 大小写转换
来源：http://spz.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://joe.shanyushiyangtech.top

[R25] 去后缀 / 去前缀
来源：http://lwd.xuetiantiany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zst.tian-w.cn

[R26] 命令替换
来源：http://gvx.zhixingplan.top

now=$(date +%F); echo "$now"
来源：http://ism.hesvh.cn

[R27] 算术展开
来源：http://tcd.sufxvd.cn

echo $((1 + 2 * 3))
来源：http://ucz.jinyuanbaomall.cn

[R28] 浮点运算
来源：http://ymc.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://ljs.sweek.top

[R29] 定义函数
来源：http://jdv.ctjpmb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://itc.tarul.cn

[R30] 函数返回状态码
来源：http://dmk.jinqigfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://ouv.yueranfly.top

[R31] 局部变量
来源：http://ecd.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://pdh.cashguo.top

[R32] 参数个数校验
来源：http://fta.ydjk.org.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nuq.gaohongyu789.top

[R33] 捕获错误并提示行号
来源：http://nkg.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ezr.vqdsnc.cn

[R34] 退出时清理
来源：http://qdm.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://iuj.9152youxi.cn

[R35] 后台执行并等待
来源：http://fku.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://vbe.aizwys.cn

[R36] 并发执行多个任务
来源：http://tah.tanke756.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ksd.gzhubu.top

[R37] 把输出赋给变量
来源：http://hcw.0kj1m.cn

files=$(ls -1)
来源：http://jfs.iojbl.cn

[R38] 管道串联
来源：http://obw.guannengcc.top

cat a.txt | grep -i error | wc -l
来源：http://uqb.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://vxv.xylfe.cn

cmd > out.log 2>&1
来源：http://val.ehwqpu.com

[R40] 追加写日志
来源：http://gbl.jinqigfzy.top

echo "log" >> out.log
来源：http://hdy.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://veh.chenjidiqi.icu

cmd >/dev/null 2>&1
来源：http://ihw.yj202588.top

[R42] 输入重定向
来源：http://vva.sweek.top

wc -l < a.txt
来源：http://wxo.sufxvd.cn

[R43] 按名字查找文件
来源：http://jnh.svipenyu.cn

find . -name "*.log" -type f
来源：http://etq.fzhhl.top

[R44] 按修改时间查找
来源：http://msa.bjfxy.top

find . -mtime -7 -type f
来源：http://spc.dianchejie.cn

[R45] 批量删除
来源：http://ljr.jqgfzy.top

find . -name "*.tmp" -delete
来源：http://ufe.jyoumei.cn

[R46] 递归替换文件内容
来源：http://dke.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bcz.jinghuilouyu.cn

[R47] sed 单行替换
来源：http://kts.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oaq.zhiwuduotai.top

[R48] awk 取指定列
来源：http://ycl.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://ivt.hnqzz.top

[R49] awk 带条件
来源：http://ivy.svipenyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yih.yfazqb.com

[R50] awk 求和
来源：http://smy.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fib.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://zaz.nanxuanxn.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ixg.mhx1999.top

[R52] 统计行数
来源：http://crr.xinyue.icu

wc -l a.txt
来源：http://fdn.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://ktx.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vdx.guannengcc.top

[R54] 比较两个文件
来源：http://kvt.tanke756.top

diff a.txt b.txt
来源：http://eoo.jiagoushi.top

[R55] 压缩与解压
来源：http://obe.cashguo.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://htl.yonumen.top

[R56] 远程拷贝
来源：http://nyv.yuanzhike.top

scp file user@host:/path/
来源：http://knv.ydjk.org.cn

[R57] 远程执行命令
来源：http://aux.yj20258.top

ssh user@host 'uptime'
来源：http://awi.ydzc1.top

[R58] 下载文件
来源：http://frq.chenlongwang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mbr.chenlongwang.top

[R59] 发 POST JSON
来源：http://gak.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xxf.gotoacloud.top

[R60] 只看 HTTP 状态码
来源：http://dfj.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sdl.hysaishi.cn

[R61] 磁盘占用
来源：http://kwm.cqqwz.cn

df -h;  du -sh *
来源：http://qkf.hywenlv.cn

[R62] 找最占空间的文件
来源：http://eii.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://moo.andypj.xyz

[R63] 内存与进程
来源：http://wlv.fanxiaobao.xyz

free -h;  ps aux | grep nginx
来源：http://uea.0kj1m.cn

[R64] 结束进程
来源：http://vhs.zhaomingkeji.xyz

kill -9 $(pgrep -f app.py)
来源：http://cll.c1oappe.top

[R65] 查看端口占用
来源：http://qeb.jiagoushi.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mvc.yonumen.top

[R66] 定时任务
来源：http://iok.jinqigfzy.top

crontab -e;  crontab -l
来源：http://yuw.jiagoushi.top

[R67] 生成随机十六进制串
来源：http://avw.xziqi.cn

openssl rand -hex 16
来源：http://lez.svipenyu.cn

[R68] 计算文件校验值
来源：http://wsx.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://wyh.dianchejie.cn

[R69] 生成随机密码
来源：http://vao.yj20258888.top

head -c 16 /dev/urandom | base64
来源：http://nkb.zhoulong.xyz

[R70] 时间戳与互转
来源：http://sig.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://fpb.xingfuxueyuan.xyz

[R71] 日期格式化
来源：http://uhj.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://erp.yj20258888.top

[R72] 等待端口就绪
来源：http://dja.guowangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://oct.cheryme.top

[R73] 分割大日志
来源：http://gnb.hesvh.cn

split -l 1000 big.log part_
来源：http://eue.xingfuxueyuan.xyz

[R74] 批量重命名
来源：http://lgl.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pgw.shangyingyoupin.top

[R75] 导出环境变量
来源：http://lcx.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://bkj.cqqwz.cn

[R76] 使用临时文件
来源：http://ynb.hnqzz.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oxd.yuxming.cn

[R77] 读取用户输入
来源：http://fjm.xingfuxueyuan.xyz

read -rp "请输入: " ans
来源：http://tnb.zdqjudy.top

[R78] 交互式菜单
来源：http://rrm.chenzaomai.com

select opt in a b c; do echo "$opt"; break; done
来源：http://vul.ybcxt.top

[R79] 解析命令行选项
来源：http://skb.zdqjudy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dod.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://wdb.sweek.top

time ./run.sh
来源：http://eju.jinghuilouyu.cn

================================================================================
来源：http://wps.zdqjudy.top

S. C / C++ 专题
来源：http://goo.ywan-chungtsiang.top

================================================================================
来源：http://nxm.vehdjk.com

[S01] C：Hello World
来源：http://exk.uphjek.com

#include <stdio.h>
来源：http://nad.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gmv.bjfxy.top

[S02] C：变量与格式化输出
来源：http://ugp.xuetiantiany.cn

int a = 10; printf("%d\n", a);
来源：http://xws.fehbvm.com

[S03] C：读入整数
来源：http://tvt.kuanghao11.cn

int x; scanf("%d", &x);
来源：http://hrk.dianchejie.cn

[S04] C：字符串复制
来源：http://oqq.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://gfw.svipenyu.cn

[S05] C：字符串长度
来源：http://lhv.c1oappe.top

strlen(s)
来源：http://qwq.quarkkingdee.top

[S06] C：字符串比较
来源：http://vfe.shangyingyoupin.top

strcmp(a, b) == 0
来源：http://zfi.aibaodan.cn

[S07] C：数组遍历求和
来源：http://nyg.dianchejie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zlw.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://bbe.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cmk.fanxiaobao.xyz

[S09] C：结构体定义与初始化
来源：http://jar.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rnl.fktsv.cn

[S10] C：指针与解引用
来源：http://myg.yueranfly.top

int *p = &a;  *p = 5;
来源：http://njr.xziqi.cn

[S11] C：逐行读文件
来源：http://cgt.redwolf501.top

FILE *f = fopen("a.txt", "r");
来源：http://xtw.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zpj.ydzc1.top

fclose(f);
来源：http://qum.hywenlv.cn

[S12] C：写文件
来源：http://rvw.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://red.yj202588.top

[S13] C：宏定义
来源：http://zvg.yueranfly.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://znu.cashguo.top

[S14] C：枚举
来源：http://utq.hammf.cn

enum Color { RED, GREEN, BLUE };
来源：http://hpg.xingfuxueyuan.xyz

[S15] C：类型转换
来源：http://aco.zdqjudy.top

(double) a / b
来源：http://hcz.zhaomingkeji.xyz

[S16] C：位操作置位
来源：http://gnm.smart0.xyz

x |= (1 << 3);
来源：http://lnu.nwbrower.top

[S17] C：安全拼接字符串
来源：http://foy.hysaishi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://apn.cheryme.top

[S18] C：命令行参数
来源：http://hau.dashuyun.cn

int main(int argc, char **argv)
来源：http://lyx.jinghuilouyu.cn

[S19] C：快速排序
来源：http://lkv.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://cwi.tarul.cn

[S20] C：二分查找
来源：http://kud.xingfuxueyuan.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mpi.iojbl.cn

[S21] C：字符类别判断
来源：http://cxu.vehdjk.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rvd.daxiang520.top

[S22] C：字符串转数字
来源：http://tau.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://brz.sysykeji.top

[S23] C：随机数
来源：http://hxb.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cjq.sysykeji.top

[S24] C：获取本地时间
来源：http://fci.jqgufenzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qhy.zhoulong.xyz

[S25] C：内存拷贝
来源：http://lrv.pycfn.com

memcpy(dst, src, n);
来源：http://hco.yj20258888.top

[S26] C：内存清零
来源：http://gku.pycfn.com

memset(a, 0, sizeof a);
来源：http://hkw.haohaochexian.top

[S27] C：定义常量
来源：http://swo.yuxming.cn

const double PI = 3.14159;
来源：http://kob.mhx1999.top

[S28] C：静态变量
来源：http://hjm.quarkkingdee.top

static int counter = 0;
来源：http://gdf.birdmap.top

[S29] C：变参函数
来源：http://mbl.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dyx.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://llt.316326.xyz

#ifndef X_H
来源：http://cfy.nanxinkj.top

#define X_H
来源：http://fqe.quarkkingdee.top

#endif
来源：http://yci.vqdsnc.cn

[S31] C++：Hello World
来源：http://ezf.zhiwuduotai.top

#include <iostream>
来源：http://hui.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://qoo.cqqwz.cn

[S32] C++：字符串
来源：http://aue.wangshuangyany.cn

std::string s = "hi";  s += "!";
来源：http://vvg.52xcode.cn

[S33] C++：vector 增删
来源：http://mvo.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jtv.zhixingplan.top

[S34] C++：遍历 vector
来源：http://prd.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://nyl.zhengqikj.top

[S35] C++：map
来源：http://uvt.yfazqb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oka.zhaomingkeji.xyz

[S36] C++：unordered_map
来源：http://fxm.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ciw.ppjwa.cn

[S37] C++：set
来源：http://tcn.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bba.ctjpmb.com

[S38] C++：排序
来源：http://vdo.redwolf501.top

std::sort(v.begin(), v.end());
来源：http://oms.zhongyouzk.top

[S39] C++：自定义比较器排序
来源：http://fgf.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lot.yj202588.top

[S40] C++：查找元素
来源：http://feu.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nqt.52xcode.cn

[S41] C++：类与构造函数
来源：http://ybn.yonumen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rlo.hnxiangtu.top

[S42] C++：继承与虚函数
来源：http://jpp.bjfxy.top

class B : public Base { public: void f() override {} };
来源：http://fmc.xziqi.cn

[S43] C++：智能指针
来源：http://iam.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://gyx.daxiang520.top

[S44] C++：引用传参
来源：http://wbk.jyoumei.cn

void inc(int &x) { ++x; }
来源：http://pad.ybcxt.top


<!-- 参考信息 -->