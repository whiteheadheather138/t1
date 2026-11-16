代发 wailian999

SHOW INDEX FROM users;
来源：http://srt.hfpthk.cn

[Q73] 查看表状态
来源：http://akh.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://whp.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://kyi.chenzaomai.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://upl.chenzaomai.com

[Q75] 日期格式化
来源：http://mfn.hnxiangtu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mfo.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kmn.nanxuanxn.top

[Q76] 按天统计
来源：http://pxx.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wce.zhiwuduotai.top

[Q77] 时间加减
来源：http://zoq.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wfw.xylfe.cn

[Q78] 当前时间
来源：http://lul.birdmap.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dkc.chenjidiqi.icu

[Q79] 字符串拼接
来源：http://wrh.hfpthk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lmu.sysykeji.top

[Q80] 字符串截取
来源：http://izo.hysaishi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://syf.cucudq.cn

[Q81] 字符串替换
来源：http://qro.dashuyun.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gmx.dashuyun.cn

[Q82] 字符长度与字节长度
来源：http://vts.yj202588.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://leq.daxiang520.top

[Q83] 大小写转换
来源：http://imh.nanxuanxn.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://miy.jianghu66.top

[Q84] 去除首尾空格
来源：http://fgf.52xcode.cn

SELECT TRIM(name) FROM users;
来源：http://bbb.jiagoushi.top

[Q85] 数值取整
来源：http://wej.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mfn.tarul.cn

[Q86] 读取 JSON 字段
来源：http://xfj.yueranfly.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jng.epnwcf.com

[Q87] JSON 字段做条件
来源：http://qok.jianghu66.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zhv.jinghuilouyu.cn

[Q88] 行转列（条件聚合）
来源：http://tyn.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qsf.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uja.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://rnq.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yaw.pycfn.com

[Q90] 生成序号列
来源：http://jbt.wangdashe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iwn.xziqi.cn

================================================================================
来源：http://etq.jinqigufen.top

R. Bash 专题
来源：http://ved.sxryk.cn

================================================================================
来源：http://jge.andypj.xyz

[R01] shebang 与严格模式
来源：http://iyq.yj20258888.top

#!/usr/bin/env bash
来源：http://ced.shangyingyoupin.top

set -euo pipefail
来源：http://xfk.ehwqpu.com

[R02] 变量赋值与使用
来源：http://bhj.haohaochexian.top

name="Tom"; echo "$name"
来源：http://jyj.wangshuangyany.cn

[R03] 只读变量
来源：http://dtn.jyoumei.cn

readonly PI=3.14
来源：http://kxo.yj20258.top

[R04] 位置参数
来源：http://joz.shangyingyoupin.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vum.yj20258888.top

[R05] 参数默认值
来源：http://mpj.jinqigufen.top

name="${1:-default}"
来源：http://erv.havefunace.top

[R06] 判断命令是否存在
来源：http://etz.quarkkingdee.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mhg.aizwys.cn

[R07] if 判断文件
来源：http://wyt.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xiz.xinyue.icu

[R08] 数值比较
来源：http://ljx.birdmap.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rpw.feifeiyinyue.top

[R09] 字符串比较
来源：http://wri.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fyg.guannengcc.top

[R10] 正则匹配
来源：http://jov.shangyingyoupin.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dps.zhoulong.xyz

[R11] case 多分支
来源：http://nwh.xingfuxueyuan.xyz

case "$1" in
来源：http://bwc.ivvv.top

start) echo "启动" ;;
来源：http://vws.yj20258888.top

stop)  echo "停止" ;;
来源：http://fba.hnqzz.top

*)     echo "未知命令" ;;
来源：http://kif.yongpay.top

esac
来源：http://rhx.chenlongwang.top

[R12] for 遍历文件
来源：http://twc.shuidangran.top

for f in *.txt; do echo "$f"; done
来源：http://ana.fktsv.cn

[R13] for 计数循环
来源：http://tho.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://gdf.316326.xyz

[R14] C 风格 for
来源：http://ckw.fehbvm.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://anz.jlsjyb.cn

[R15] while 逐行读文件
来源：http://xhe.xingfuxueyuan.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pkv.guannengcc.top

[R16] until 等待条件
来源：http://vlr.fktsv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tgr.xziqi.cn

[R17] 数组定义与取值
来源：http://ere.nanxuanxn.top

arr=(a b c); echo "${arr[0]}"
来源：http://tpj.hnqzz.top

[R18] 遍历数组
来源：http://ltb.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gtj.zhengqikj.top

[R19] 数组长度
来源：http://blf.ehwqpu.com

echo "${#arr[@]}"
来源：http://kee.jinghuilouyu.cn

[R20] 关联数组（字典）
来源：http://hdj.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fxv.sxryk.cn

[R21] 字符串长度
来源：http://mdd.yj20258888.top

echo "${#s}"
来源：http://cuk.chenzaomai.com

[R22] 截取子串
来源：http://ide.nanxuanxn.top

echo "${s:0:5}"
来源：http://tkn.yueranfly.top

[R23] 字符串替换
来源：http://ing.zhengqikj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rwx.jinyuanbaomall.cn

[R24] 大小写转换
来源：http://vwf.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gew.52xcode.cn

[R25] 去后缀 / 去前缀
来源：http://ult.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lwb.wangdashe.top

[R26] 命令替换
来源：http://fii.havefunace.top

now=$(date +%F); echo "$now"
来源：http://qsl.fzhhl.top

[R27] 算术展开
来源：http://wvy.jinyuanbaomall.cn

echo $((1 + 2 * 3))
来源：http://jpj.hfpthk.cn

[R28] 浮点运算
来源：http://gsx.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://ukx.nanxinkj.top

[R29] 定义函数
来源：http://opi.cashguo.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fds.epnwcf.com

[R30] 函数返回状态码
来源：http://cep.jqgfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://vti.andypj.xyz

[R31] 局部变量
来源：http://unx.andypj.xyz

f() { local x=1; echo "$x"; }
来源：http://epk.xinyue.icu

[R32] 参数个数校验
来源：http://jfu.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pqz.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://dyj.c1oappe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vca.dashuyun.cn

[R34] 退出时清理
来源：http://ndu.zhaomingkeji.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://cwc.52xcode.cn

[R35] 后台执行并等待
来源：http://oof.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jth.shuidangran.top

[R36] 并发执行多个任务
来源：http://kcq.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ntx.zycfv.cn

[R37] 把输出赋给变量
来源：http://yes.fengsongda.top

files=$(ls -1)
来源：http://luw.nanxinkj.top

[R38] 管道串联
来源：http://zds.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://qjk.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://gea.hnxiangtu.top

cmd > out.log 2>&1
来源：http://iye.nanxuanxn.top

[R40] 追加写日志
来源：http://hcj.kuanghao11.cn

echo "log" >> out.log
来源：http://vch.mhx1999.top

[R41] 丢弃输出
来源：http://xcd.hnxiangtu.top

cmd >/dev/null 2>&1
来源：http://czl.ehwqpu.com

[R42] 输入重定向
来源：http://bim.hywenlv.cn

wc -l < a.txt
来源：http://kxv.gotoacloud.top

[R43] 按名字查找文件
来源：http://dwd.aibaodan.cn

find . -name "*.log" -type f
来源：http://flj.yvedp.cn

[R44] 按修改时间查找
来源：http://ugg.hcnkem.com

find . -mtime -7 -type f
来源：http://zno.chenlongwang.top

[R45] 批量删除
来源：http://lvj.redwolf501.top

find . -name "*.tmp" -delete
来源：http://kne.jqgfzy.top

[R46] 递归替换文件内容
来源：http://siz.tarul.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kxc.epnwcf.com

[R47] sed 单行替换
来源：http://xbw.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ynf.c1oappe.top

[R48] awk 取指定列
来源：http://cbq.xuanzx.com

awk '{print $1, $3}' a.txt
来源：http://kco.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://uys.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yep.zhaomingkeji.xyz

[R50] awk 求和
来源：http://gfd.yj20258888.top

awk '{s += $2} END {print s}' a.txt
来源：http://kam.xingfuxueyuan.xyz

[R51] 排序去重取前几
来源：http://xho.redwolf501.top

sort a.txt | uniq -c | sort -rn | head
来源：http://sfw.tian-w.cn

[R52] 统计行数
来源：http://fzl.aizwys.cn

wc -l a.txt
来源：http://ssj.bjfxy.top

[R53] 查看文件头与实时尾
来源：http://jmw.ctjpmb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nwd.vqdsnc.cn

[R54] 比较两个文件
来源：http://src.ydjk.org.cn

diff a.txt b.txt
来源：http://zga.sjlbkw.cn

[R55] 压缩与解压
来源：http://cgn.birdmap.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://esx.xuetiantiany.cn

[R56] 远程拷贝
来源：http://qst.ivvv.top

scp file user@host:/path/
来源：http://zlj.wangdashe.top

[R57] 远程执行命令
来源：http://hcy.316326.xyz

ssh user@host 'uptime'
来源：http://axz.52xcode.cn

[R58] 下载文件
来源：http://uep.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ozg.jinqigufen.top

[R59] 发 POST JSON
来源：http://uzg.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fww.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://cqs.xuetiantiany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://awq.shanyushiyangkeji.top

[R61] 磁盘占用
来源：http://zgy.bbcook.cn

df -h;  du -sh *
来源：http://zep.jiagoushi.top

[R62] 找最占空间的文件
来源：http://fzf.haohaochexian.top

du -ah . | sort -rh | head -10
来源：http://quv.ctjpmb.com

[R63] 内存与进程
来源：http://upf.0kj1m.cn

free -h;  ps aux | grep nginx
来源：http://xxz.dashuyun.cn

[R64] 结束进程
来源：http://kjg.jqgfzy.top

kill -9 $(pgrep -f app.py)
来源：http://ozo.zhongyouzk.top

[R65] 查看端口占用
来源：http://iwr.iojbl.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qhc.chenjidiqi.icu

[R66] 定时任务
来源：http://vwx.hnxiangtu.top

crontab -e;  crontab -l
来源：http://bdk.zdqjudy.top

[R67] 生成随机十六进制串
来源：http://tkv.jinghuilouyu.cn

openssl rand -hex 16
来源：http://lyh.xinyue.icu

[R68] 计算文件校验值
来源：http://nsh.zdbjq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xhk.bbcook.cn

[R69] 生成随机密码
来源：http://xws.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://azj.fehbvm.com

[R70] 时间戳与互转
来源：http://sgk.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://ohi.gzhubu.top

[R71] 日期格式化
来源：http://gaz.hcnkem.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://pxf.ppjwa.cn

[R72] 等待端口就绪
来源：http://lby.yj20258888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hqf.hywenlv.cn

[R73] 分割大日志
来源：http://vyt.zhixingplan.top

split -l 1000 big.log part_
来源：http://rqn.shzxlz.cn

[R74] 批量重命名
来源：http://wmi.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zxr.gaohongyu789.top

[R75] 导出环境变量
来源：http://xws.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://bfs.cdnleiting.top

[R76] 使用临时文件
来源：http://gef.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gzh.jianghu66.top

[R77] 读取用户输入
来源：http://rqo.hfpthk.cn

read -rp "请输入: " ans
来源：http://gxm.shangyingyoupin.top

[R78] 交互式菜单
来源：http://czh.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://who.aibaodan.cn

[R79] 解析命令行选项
来源：http://ghx.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uif.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://qgg.tarul.cn

time ./run.sh
来源：http://cbv.sxryk.cn

================================================================================
来源：http://kgp.chenjidiqi.icu

S. C / C++ 专题
来源：http://hww.zhijiandao.cn

================================================================================
来源：http://bwb.tarul.cn

[S01] C：Hello World
来源：http://hiq.zdqjudy.top

#include <stdio.h>
来源：http://rqg.sufxvd.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ktx.yj202588.top

[S02] C：变量与格式化输出
来源：http://cyt.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://hgg.ydzc1.top

[S03] C：读入整数
来源：http://ajb.cheryme.top

int x; scanf("%d", &x);
来源：http://gsc.svipenyu.cn

[S04] C：字符串复制
来源：http://tyy.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://wsr.vehdjk.com

[S05] C：字符串长度
来源：http://qaa.yangfankeji.com

strlen(s)
来源：http://lqp.xinyue.icu

[S06] C：字符串比较
来源：http://hba.meibo888.top

strcmp(a, b) == 0
来源：http://jck.hnxiangtu.top

[S07] C：数组遍历求和
来源：http://ahf.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fue.0kj1m.cn

[S08] C：动态内存分配与释放
来源：http://sho.gaohongyu789.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zcs.jlsjyb.cn

[S09] C：结构体定义与初始化
来源：http://dqf.jqgufenzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://znc.yj20258888.top

[S10] C：指针与解引用
来源：http://iae.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://ubb.snrcjt.cn

[S11] C：逐行读文件
来源：http://tev.hongshengwenyu.top

FILE *f = fopen("a.txt", "r");
来源：http://ydg.meibo888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://iqz.xylfe.cn

fclose(f);
来源：http://dld.tarul.cn

[S12] C：写文件
来源：http://xyt.cdnleiting.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mqq.jiagoushi.top

[S13] C：宏定义
来源：http://qiz.zhixingplan.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jxt.havefunace.top

[S14] C：枚举
来源：http://ino.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://mer.zycfv.cn

[S15] C：类型转换
来源：http://gfz.sysykeji.top

(double) a / b
来源：http://fga.hcnkem.com

[S16] C：位操作置位
来源：http://xol.sweek.top

x |= (1 << 3);
来源：http://sjq.ctjpmb.com

[S17] C：安全拼接字符串
来源：http://iye.zhongyouzk.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nxu.52xcode.cn

[S18] C：命令行参数
来源：http://ams.0kj1m.cn

int main(int argc, char **argv)
来源：http://fir.fengsongda.top

[S19] C：快速排序
来源：http://xom.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://gbl.vehdjk.com

[S20] C：二分查找
来源：http://ggk.uphjek.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qxa.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://ceg.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yki.cqqwz.cn

[S22] C：字符串转数字
来源：http://yxa.cqqwz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://weg.jinyuanbaomall.cn

[S23] C：随机数
来源：http://xiq.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://tbm.zhijiandao.cn

[S24] C：获取本地时间
来源：http://mlc.fktsv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ppe.guannengcc.top

[S25] C：内存拷贝
来源：http://bfi.svipenyu.cn

memcpy(dst, src, n);
来源：http://ycs.sxryk.cn

[S26] C：内存清零
来源：http://dmq.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://keu.xuetiantiany.cn

[S27] C：定义常量
来源：http://vcr.dashuyun.cn

const double PI = 3.14159;
来源：http://vjg.andypj.xyz

[S28] C：静态变量
来源：http://jle.nwbrower.top

static int counter = 0;
来源：http://djx.xuanzx.com

[S29] C：变参函数
来源：http://acd.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rko.316326.xyz

[S30] C：头文件保护
来源：http://lqf.zhiwuduotai.top

#ifndef X_H
来源：http://qfh.cdnleiting.top

#define X_H
来源：http://omf.snrcjt.cn

#endif
来源：http://wyk.fzhhl.top

[S31] C++：Hello World
来源：http://pti.shanyushiyangkeji.top

#include <iostream>
来源：http://mdy.wangdashe.top

int main() { std::cout << "Hello\n"; }
来源：http://srd.ydjk.org.cn

[S32] C++：字符串
来源：http://zcu.meibo888.top

std::string s = "hi";  s += "!";
来源：http://axw.jinqigfzy.top

[S33] C++：vector 增删
来源：http://pnm.aizwys.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yze.dashuyun.cn

[S34] C++：遍历 vector
来源：http://ber.hysaishi.cn

for (auto &x : v) { std::cout << x; }
来源：http://egz.c1oappe.top

[S35] C++：map
来源：http://xmy.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kjr.epnwcf.com

[S36] C++：unordered_map
来源：http://ois.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tos.ppjwa.cn

[S37] C++：set
来源：http://vxu.jqgufenzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ehh.cqqwz.cn

[S38] C++：排序
来源：http://wbz.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://hqa.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://ayt.pycfn.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wok.snrcjt.cn

[S40] C++：查找元素
来源：http://git.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ago.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://qrj.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rrl.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://imx.guannengcc.top

class B : public Base { public: void f() override {} };
来源：http://sbh.fzhhl.top


<!-- 参考信息 -->