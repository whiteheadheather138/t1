代发 wailian999

ROLLBACK TO sp1;
来源：http://eoc.tanke756.top

[Q69] 查看执行计划
来源：http://okf.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qoh.yanxiufei.cn

[Q70] 更新统计信息
来源：http://mug.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://vsk.cqqwz.cn

[Q71] 查看建表语句
来源：http://sqa.hesvh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bfn.guowangkeji.top

[Q72] 查看索引
来源：http://fsm.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://oec.yongpay.top

[Q73] 查看表状态
来源：http://qwq.hammf.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qnn.ywan-chungtsiang.top

[Q74] 强制使用索引
来源：http://ewc.pengpengdd.cyou

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rns.yfazqb.com

[Q75] 日期格式化
来源：http://eev.hywenlv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zbn.nwbrower.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://obb.birdmap.top

[Q76] 按天统计
来源：http://ora.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qcx.pycfn.com

[Q77] 时间加减
来源：http://kqb.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tjc.9152youxi.cn

[Q78] 当前时间
来源：http://mgr.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nqj.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://psa.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uie.cheryme.top

[Q80] 字符串截取
来源：http://whx.dianchejie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wzj.shanyushiyangkeji.top

[Q81] 字符串替换
来源：http://wux.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bvl.zdqjudy.top

[Q82] 字符长度与字节长度
来源：http://nej.jlsjyb.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cmp.ydzc1.top

[Q83] 大小写转换
来源：http://fbf.hywenlv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uji.fzhhl.top

[Q84] 去除首尾空格
来源：http://oms.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://paz.zdqjudy.top

[Q85] 数值取整
来源：http://pnq.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zzz.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://jvm.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ngp.yanxiufei.cn

[Q87] JSON 字段做条件
来源：http://oko.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xkh.wangshuangyany.cn

[Q88] 行转列（条件聚合）
来源：http://zud.yonumen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tfk.havefunace.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nea.xylfe.cn

[Q89] 判断表是否存在
来源：http://dnz.havefunace.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bzf.redwolf501.top

[Q90] 生成序号列
来源：http://bhi.sjlbkw.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mtn.hnxiangtu.top

================================================================================
来源：http://mkl.fengsongda.top

R. Bash 专题
来源：http://own.ppjwa.cn

================================================================================
来源：http://vqx.havefunace.top

[R01] shebang 与严格模式
来源：http://uqa.ivvv.top

#!/usr/bin/env bash
来源：http://rpq.jianghu66.top

set -euo pipefail
来源：http://ccl.yuxming.cn

[R02] 变量赋值与使用
来源：http://hxt.aizwys.cn

name="Tom"; echo "$name"
来源：http://ftv.hcnkem.com

[R03] 只读变量
来源：http://wba.fengsongda.top

readonly PI=3.14
来源：http://ztl.sjlbkw.cn

[R04] 位置参数
来源：http://pqu.shanyushiyangtech.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jdk.yanxiufei.cn

[R05] 参数默认值
来源：http://zft.ctjpmb.com

name="${1:-default}"
来源：http://eky.cucudq.cn

[R06] 判断命令是否存在
来源：http://rop.xuetiantiany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bzh.wangshuangyany.cn

[R07] if 判断文件
来源：http://cyf.sjlbkw.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lim.xuanzx.com

[R08] 数值比较
来源：http://fxd.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://chq.ydjk.org.cn

[R09] 字符串比较
来源：http://rar.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eix.zycfv.cn

[R10] 正则匹配
来源：http://kpy.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ayv.pengpengdd.cyou

[R11] case 多分支
来源：http://wuz.ydjk.org.cn

case "$1" in
来源：http://xni.ppjwa.cn

start) echo "启动" ;;
来源：http://bcb.yangfankeji.com

stop)  echo "停止" ;;
来源：http://sgy.yonumen.top

*)     echo "未知命令" ;;
来源：http://bdy.jianghu66.top

esac
来源：http://vwm.epnwcf.com

[R12] for 遍历文件
来源：http://kol.yvedp.cn

for f in *.txt; do echo "$f"; done
来源：http://bgr.tarul.cn

[R13] for 计数循环
来源：http://pmu.jinghuilouyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://qsp.chenjidiqi.icu

[R14] C 风格 for
来源：http://ach.xinyue.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jvo.cqqwz.cn

[R15] while 逐行读文件
来源：http://dlp.dashuyun.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://afi.xylfe.cn

[R16] until 等待条件
来源：http://rjl.9152youxi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eoz.52xcode.cn

[R17] 数组定义与取值
来源：http://wto.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://bmm.quarkkingdee.top

[R18] 遍历数组
来源：http://jpp.quarkkingdee.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rxn.gaohongyu789.top

[R19] 数组长度
来源：http://vor.birdmap.top

echo "${#arr[@]}"
来源：http://uim.hnqzz.top

[R20] 关联数组（字典）
来源：http://cuo.iojbl.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fbv.c1oappe.top

[R21] 字符串长度
来源：http://xdl.uphjek.com

echo "${#s}"
来源：http://elw.gzhubu.top

[R22] 截取子串
来源：http://fla.c1oappe.top

echo "${s:0:5}"
来源：http://lob.cdnleiting.top

[R23] 字符串替换
来源：http://njo.daria6918.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uzk.yj202588.top

[R24] 大小写转换
来源：http://mxw.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jpj.jinghuilouyu.cn

[R25] 去后缀 / 去前缀
来源：http://gtv.yj20258.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gen.yangfankeji.com

[R26] 命令替换
来源：http://nqk.jlsjyb.cn

now=$(date +%F); echo "$now"
来源：http://cai.zhijiandao.cn

[R27] 算术展开
来源：http://zzk.aizwys.cn

echo $((1 + 2 * 3))
来源：http://xuk.yuxming.cn

[R28] 浮点运算
来源：http://rrn.sxryk.cn

echo "scale=2; 10/3" | bc
来源：http://ukz.hcnkem.com

[R29] 定义函数
来源：http://ggl.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bkw.jinghuilouyu.cn

[R30] 函数返回状态码
来源：http://kte.jinqigfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://jnj.jianghu66.top

[R31] 局部变量
来源：http://uys.aizwys.cn

f() { local x=1; echo "$x"; }
来源：http://dvl.nwbrower.top

[R32] 参数个数校验
来源：http://sww.ctjpmb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bej.xuetiantiany.cn

[R33] 捕获错误并提示行号
来源：http://cct.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lxp.yj20258888.top

[R34] 退出时清理
来源：http://mfw.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://joo.jlsjyb.cn

[R35] 后台执行并等待
来源：http://rkr.xinyue.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://cpm.cdnleiting.top

[R36] 并发执行多个任务
来源：http://men.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cmd.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://fof.zdbjq.cn

files=$(ls -1)
来源：http://nos.dashuyun.cn

[R38] 管道串联
来源：http://aaq.gotoacloud.top

cat a.txt | grep -i error | wc -l
来源：http://btn.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://wjl.jlsjyb.cn

cmd > out.log 2>&1
来源：http://xnz.gotoacloud.top

[R40] 追加写日志
来源：http://imz.yangfankeji.com

echo "log" >> out.log
来源：http://wyr.hnqzz.top

[R41] 丢弃输出
来源：http://pjm.xylfe.cn

cmd >/dev/null 2>&1
来源：http://mht.zycfv.cn

[R42] 输入重定向
来源：http://lns.smart0.xyz

wc -l < a.txt
来源：http://iqj.xinyue.icu

[R43] 按名字查找文件
来源：http://ihu.feifeiyinyue.top

find . -name "*.log" -type f
来源：http://ezg.bjfxy.top

[R44] 按修改时间查找
来源：http://xvy.yueranfly.top

find . -mtime -7 -type f
来源：http://uum.chenzaomai.com

[R45] 批量删除
来源：http://yqb.yj202588.top

find . -name "*.tmp" -delete
来源：http://tba.jianghu66.top

[R46] 递归替换文件内容
来源：http://iku.0kj1m.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dcn.chenzaomai.com

[R47] sed 单行替换
来源：http://irg.zhengqikj.top

sed -i 's/foo/bar/g' a.txt
来源：http://kpa.gaohongyu789.top

[R48] awk 取指定列
来源：http://lmx.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://gir.cdnleiting.top

[R49] awk 带条件
来源：http://fsw.yuanzhike.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://klh.gotoacloud.top

[R50] awk 求和
来源：http://wrd.gotoacloud.top

awk '{s += $2} END {print s}' a.txt
来源：http://acj.jinqigfzy.top

[R51] 排序去重取前几
来源：http://hbn.c1oappe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ckh.tianlin.xyz

[R52] 统计行数
来源：http://ovy.tian-w.cn

wc -l a.txt
来源：http://lza.sjlbkw.cn

[R53] 查看文件头与实时尾
来源：http://oeq.zhongyouzk.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jue.mhx1999.top

[R54] 比较两个文件
来源：http://dnc.zhoulong.xyz

diff a.txt b.txt
来源：http://yay.tanke756.top

[R55] 压缩与解压
来源：http://zch.mhx1999.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cbq.sxryk.cn

[R56] 远程拷贝
来源：http://pqy.zhongyouzk.top

scp file user@host:/path/
来源：http://bky.ctjpmb.com

[R57] 远程执行命令
来源：http://mae.feifeiyinyue.top

ssh user@host 'uptime'
来源：http://yza.yj20258888.top

[R58] 下载文件
来源：http://uev.kuanghao11.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fwt.shangyingyoupin.top

[R59] 发 POST JSON
来源：http://gcu.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jtd.gotoacloud.top

[R60] 只看 HTTP 状态码
来源：http://kyo.svipenyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jwn.jinyuanbaomall.cn

[R61] 磁盘占用
来源：http://vuh.yuanzhike.top

df -h;  du -sh *
来源：http://trx.fanxiaobao.xyz

[R62] 找最占空间的文件
来源：http://qid.yongpay.top

du -ah . | sort -rh | head -10
来源：http://ult.zhengqikj.top

[R63] 内存与进程
来源：http://bft.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://adt.feifeiyinyue.top

[R64] 结束进程
来源：http://zae.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://fdl.cheryme.top

[R65] 查看端口占用
来源：http://kzz.zdqjudy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cse.316326.xyz

[R66] 定时任务
来源：http://gvp.birdmap.top

crontab -e;  crontab -l
来源：http://vac.yonumen.top

[R67] 生成随机十六进制串
来源：http://dae.jyoumei.cn

openssl rand -hex 16
来源：http://ubw.xuanzx.com

[R68] 计算文件校验值
来源：http://afb.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://wqw.havefunace.top

[R69] 生成随机密码
来源：http://clf.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://qtq.yangfankeji.com

[R70] 时间戳与互转
来源：http://sxx.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://bhr.epnwcf.com

[R71] 日期格式化
来源：http://hlz.chenjidiqi.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://qdt.yj202588.top

[R72] 等待端口就绪
来源：http://oge.wangdashe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ycg.nanxuanxn.top

[R73] 分割大日志
来源：http://gaa.ivvv.top

split -l 1000 big.log part_
来源：http://haf.yvedp.cn

[R74] 批量重命名
来源：http://wpe.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jfl.cqqwz.cn

[R75] 导出环境变量
来源：http://zrr.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://rzu.vehdjk.com

[R76] 使用临时文件
来源：http://cxr.ybcxt.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sbi.gzhubu.top

[R77] 读取用户输入
来源：http://mos.hesvh.cn

read -rp "请输入: " ans
来源：http://ikq.jlsjyb.cn

[R78] 交互式菜单
来源：http://bje.bbcook.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tvf.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://gzp.snrcjt.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://scs.zhaomingkeji.xyz

[R80] 查看脚本执行耗时
来源：http://pqc.ctjpmb.com

time ./run.sh
来源：http://gxk.yangfankeji.com

================================================================================
来源：http://wdx.cheryme.top

S. C / C++ 专题
来源：http://hbt.sweek.top

================================================================================
来源：http://nnh.52xcode.cn

[S01] C：Hello World
来源：http://azb.yj20258.top

#include <stdio.h>
来源：http://xfs.kuanghao11.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wbf.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://vly.nanxuanxn.top

int a = 10; printf("%d\n", a);
来源：http://nus.sysykeji.top

[S03] C：读入整数
来源：http://osx.yuxming.cn

int x; scanf("%d", &x);
来源：http://qxt.ydjk.org.cn

[S04] C：字符串复制
来源：http://dzk.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://orz.vqdsnc.cn

[S05] C：字符串长度
来源：http://vsj.52xcode.cn

strlen(s)
来源：http://dkv.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://iqy.chenzaomai.com

strcmp(a, b) == 0
来源：http://mww.gotoacloud.top

[S07] C：数组遍历求和
来源：http://crr.aibaodan.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ahw.sxryk.cn

[S08] C：动态内存分配与释放
来源：http://jxe.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://njs.hcnkem.com

[S09] C：结构体定义与初始化
来源：http://gkq.jinqigfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hqr.ywan-chungtsiang.top

[S10] C：指针与解引用
来源：http://wnz.cashguo.top

int *p = &a;  *p = 5;
来源：http://iew.hammf.cn

[S11] C：逐行读文件
来源：http://zra.pycfn.com

FILE *f = fopen("a.txt", "r");
来源：http://znd.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xmj.zhaomingkeji.xyz

fclose(f);
来源：http://nsz.cdnleiting.top

[S12] C：写文件
来源：http://oes.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lkk.snrcjt.cn

[S13] C：宏定义
来源：http://rzm.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sug.yangfankeji.com

[S14] C：枚举
来源：http://hkw.ybcxt.top

enum Color { RED, GREEN, BLUE };
来源：http://jez.yj202588.top

[S15] C：类型转换
来源：http://wnu.ybcxt.top

(double) a / b
来源：http://nbb.cdnleiting.top

[S16] C：位操作置位
来源：http://uky.mhx1999.top

x |= (1 << 3);
来源：http://asx.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://fda.xylfe.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fiy.cucudq.cn

[S18] C：命令行参数
来源：http://bgl.zdbjq.cn

int main(int argc, char **argv)
来源：http://gox.havefunace.top

[S19] C：快速排序
来源：http://qzm.fanxiaobao.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://blq.kuanghao11.cn

[S20] C：二分查找
来源：http://ntr.epnwcf.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nyl.iojbl.cn

[S21] C：字符类别判断
来源：http://twc.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jro.sysykeji.top

[S22] C：字符串转数字
来源：http://kmd.ywan-chungtsiang.top

atoi("42");  strtod("3.14", NULL);
来源：http://rce.gogol.net.cn

[S23] C：随机数
来源：http://inf.jinqigfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lbv.jinqigfzy.top

[S24] C：获取本地时间
来源：http://hov.zhijiandao.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oqm.nanxinkj.top

[S25] C：内存拷贝
来源：http://mug.sweek.top

memcpy(dst, src, n);
来源：http://ohd.jiagoushi.top

[S26] C：内存清零
来源：http://teb.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://ffk.feifeiyinyue.top

[S27] C：定义常量
来源：http://xrj.vqdsnc.cn

const double PI = 3.14159;
来源：http://pgl.gaohongyu789.top

[S28] C：静态变量
来源：http://yor.fanxiaobao.xyz

static int counter = 0;
来源：http://oid.9152youxi.cn

[S29] C：变参函数
来源：http://yyi.shanyushiyangtech.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fqu.9152youxi.cn

[S30] C：头文件保护
来源：http://jlv.cheryme.top

#ifndef X_H
来源：http://lbk.vehdjk.com

#define X_H
来源：http://uqz.meibo888.top

#endif
来源：http://ndz.chenlongwang.top

[S31] C++：Hello World
来源：http://uos.nanxuanxn.top

#include <iostream>
来源：http://jym.hnqzz.top

int main() { std::cout << "Hello\n"; }
来源：http://xiz.feifeiyinyue.top

[S32] C++：字符串
来源：http://jus.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://hnw.gogol.net.cn

[S33] C++：vector 增删
来源：http://hhu.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hmv.cashguo.top

[S34] C++：遍历 vector
来源：http://xsu.jinghuilouyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://zrb.zhiwuduotai.top

[S35] C++：map
来源：http://nsh.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://svt.shuidangran.top

[S36] C++：unordered_map
来源：http://hso.vehdjk.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ipr.ehwqpu.com

[S37] C++：set
来源：http://hkw.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ugn.cashguo.top

[S38] C++：排序
来源：http://ufw.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://vra.zhijiandao.cn


<!-- 参考信息 -->