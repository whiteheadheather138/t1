代发 wailian999

[Q67] 设置隔离级别
来源：http://fbx.snrcjt.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xgg.hnqzz.top

[Q68] 保存点
来源：http://ady.ybcxt.top

SAVEPOINT sp1;
来源：http://umd.jinqigfzy.top

ROLLBACK TO sp1;
来源：http://iey.hywenlv.cn

[Q69] 查看执行计划
来源：http://kax.daxiang520.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uun.tian-w.cn

[Q70] 更新统计信息
来源：http://aqe.zhijiandao.cn

ANALYZE TABLE users;
来源：http://rzf.bbcook.cn

[Q71] 查看建表语句
来源：http://rzh.bbcook.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iin.zhoulong.xyz

[Q72] 查看索引
来源：http://clc.316326.xyz

SHOW INDEX FROM users;
来源：http://orr.ctjpmb.com

[Q73] 查看表状态
来源：http://qet.smart0.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://tje.snrcjt.cn

[Q74] 强制使用索引
来源：http://hzf.yvedp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ruf.hesvh.cn

[Q75] 日期格式化
来源：http://mhf.cashguo.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://obm.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vji.yongpay.top

[Q76] 按天统计
来源：http://hvb.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bmx.chenjidiqi.icu

[Q77] 时间加减
来源：http://xcu.andypj.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://giw.pycfn.com

[Q78] 当前时间
来源：http://rjw.cheryme.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fob.chenzaomai.com

[Q79] 字符串拼接
来源：http://qbk.pycfn.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wmg.zhiwuduotai.top

[Q80] 字符串截取
来源：http://hpi.smart0.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oiu.cheryme.top

[Q81] 字符串替换
来源：http://bxb.nwbrower.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qwp.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://uav.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://idk.shzxlz.cn

[Q83] 大小写转换
来源：http://smc.wangdashe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vhe.ivvv.top

[Q84] 去除首尾空格
来源：http://hqd.xinyue.icu

SELECT TRIM(name) FROM users;
来源：http://htr.iojbl.cn

[Q85] 数值取整
来源：http://ejf.sweek.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://utx.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://yqh.zycfv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://puu.316326.xyz

[Q87] JSON 字段做条件
来源：http://lwd.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xyp.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://vto.yvedp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oru.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hun.yfazqb.com

[Q89] 判断表是否存在
来源：http://rin.yanxiufei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xsw.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://umj.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ifo.cucudq.cn

================================================================================
来源：http://prg.xziqi.cn

R. Bash 专题
来源：http://gfj.ydzc1.top

================================================================================
来源：http://ttt.iojbl.cn

[R01] shebang 与严格模式
来源：http://fhu.cucudq.cn

#!/usr/bin/env bash
来源：http://nac.ehwqpu.com

set -euo pipefail
来源：http://rfg.ppjwa.cn

[R02] 变量赋值与使用
来源：http://mdb.yuanzhike.top

name="Tom"; echo "$name"
来源：http://hpy.fzhhl.top

[R03] 只读变量
来源：http://mtn.dashuyun.cn

readonly PI=3.14
来源：http://xrv.jyoumei.cn

[R04] 位置参数
来源：http://fxa.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gfj.jinghuilouyu.cn

[R05] 参数默认值
来源：http://vsx.yuanzhike.top

name="${1:-default}"
来源：http://vba.aibaodan.cn

[R06] 判断命令是否存在
来源：http://ctf.kuanghao11.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blx.hysaishi.cn

[R07] if 判断文件
来源：http://mrk.redwolf501.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dak.dianchejie.cn

[R08] 数值比较
来源：http://nur.bjfxy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rri.wangshuangyany.cn

[R09] 字符串比较
来源：http://uvh.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pdq.nanxinkj.top

[R10] 正则匹配
来源：http://xky.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oot.sxryk.cn

[R11] case 多分支
来源：http://pqu.quarkkingdee.top

case "$1" in
来源：http://jvx.meibo888.top

start) echo "启动" ;;
来源：http://gpa.xziqi.cn

stop)  echo "停止" ;;
来源：http://hsk.zhengqikj.top

*)     echo "未知命令" ;;
来源：http://gjh.ybcxt.top

esac
来源：http://oqd.epnwcf.com

[R12] for 遍历文件
来源：http://jrd.9152youxi.cn

for f in *.txt; do echo "$f"; done
来源：http://zcv.yj202588.top

[R13] for 计数循环
来源：http://ptk.xuanzx.com

for i in {1..10}; do echo "$i"; done
来源：http://gox.fehbvm.com

[R14] C 风格 for
来源：http://bva.nanxinkj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mjm.dianchejie.cn

[R15] while 逐行读文件
来源：http://rxe.pengpengdd.cyou

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ack.hammf.cn

[R16] until 等待条件
来源：http://eji.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zdg.hammf.cn

[R17] 数组定义与取值
来源：http://gze.yueranfly.top

arr=(a b c); echo "${arr[0]}"
来源：http://oif.yangfankeji.com

[R18] 遍历数组
来源：http://tsj.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://orp.tarul.cn

[R19] 数组长度
来源：http://coa.hysaishi.cn

echo "${#arr[@]}"
来源：http://zhv.ctjpmb.com

[R20] 关联数组（字典）
来源：http://qdo.wangshuangyany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hzo.cdnleiting.top

[R21] 字符串长度
来源：http://byt.yonumen.top

echo "${#s}"
来源：http://dht.sysykeji.top

[R22] 截取子串
来源：http://frz.guowangkeji.top

echo "${s:0:5}"
来源：http://yiq.hongshengwenyu.top

[R23] 字符串替换
来源：http://tlo.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sgi.zhixingplan.top

[R24] 大小写转换
来源：http://vyf.sysykeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://hga.yueranfly.top

[R25] 去后缀 / 去前缀
来源：http://czq.ctjpmb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://gfx.fktsv.cn

[R26] 命令替换
来源：http://nzq.nanxuanxn.top

now=$(date +%F); echo "$now"
来源：http://gsy.cheryme.top

[R27] 算术展开
来源：http://gwn.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://qih.xylfe.cn

[R28] 浮点运算
来源：http://wwu.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://tpu.zhiwuduotai.top

[R29] 定义函数
来源：http://bwn.zhongyouzk.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nks.epnwcf.com

[R30] 函数返回状态码
来源：http://ycx.bbcook.cn

f() { return 0; }; f || echo "失败了"
来源：http://rzs.gogol.net.cn

[R31] 局部变量
来源：http://srq.0kj1m.cn

f() { local x=1; echo "$x"; }
来源：http://dwd.zhengqikj.top

[R32] 参数个数校验
来源：http://xal.xuanzx.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wnp.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://npf.jinghuilouyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dcy.xuetiantiany.cn

[R34] 退出时清理
来源：http://bai.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://iqk.hnxiangtu.top

[R35] 后台执行并等待
来源：http://idc.jqgfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wuq.sjlbkw.cn

[R36] 并发执行多个任务
来源：http://msn.iojbl.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hye.hammf.cn

[R37] 把输出赋给变量
来源：http://emd.52xcode.cn

files=$(ls -1)
来源：http://tfv.jinqigufen.top

[R38] 管道串联
来源：http://ayq.nanxinkj.top

cat a.txt | grep -i error | wc -l
来源：http://qpz.hnqzz.top

[R39] 重定向标准输出与错误
来源：http://vus.zdqjudy.top

cmd > out.log 2>&1
来源：http://jnb.fanxiaobao.xyz

[R40] 追加写日志
来源：http://rgh.cqqwz.cn

echo "log" >> out.log
来源：http://vdy.chenzaomai.com

[R41] 丢弃输出
来源：http://ute.ydzc1.top

cmd >/dev/null 2>&1
来源：http://mfk.hnxiangtu.top

[R42] 输入重定向
来源：http://yqs.yangfankeji.com

wc -l < a.txt
来源：http://jsi.zycfv.cn

[R43] 按名字查找文件
来源：http://rls.hysaishi.cn

find . -name "*.log" -type f
来源：http://efr.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://lrv.sufxvd.cn

find . -mtime -7 -type f
来源：http://wzz.xylfe.cn

[R45] 批量删除
来源：http://qwb.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://wlb.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://gmx.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sru.andypj.xyz

[R47] sed 单行替换
来源：http://mnx.andypj.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://rcx.shangyingyoupin.top

[R48] awk 取指定列
来源：http://rpb.jinqigufen.top

awk '{print $1, $3}' a.txt
来源：http://xzm.jiagoushi.top

[R49] awk 带条件
来源：http://fhw.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jks.svipenyu.cn

[R50] awk 求和
来源：http://kfe.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tkf.zhoulong.xyz

[R51] 排序去重取前几
来源：http://ghx.xylfe.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zfi.cqqwz.cn

[R52] 统计行数
来源：http://dje.hfpthk.cn

wc -l a.txt
来源：http://zog.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://dtn.ehwqpu.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kbo.jqgfzy.top

[R54] 比较两个文件
来源：http://lsp.chenlongwang.top

diff a.txt b.txt
来源：http://oks.zycfv.cn

[R55] 压缩与解压
来源：http://cgu.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ebx.c1oappe.top

[R56] 远程拷贝
来源：http://nsd.epnwcf.com

scp file user@host:/path/
来源：http://gsl.tarul.cn

[R57] 远程执行命令
来源：http://mzs.gogol.net.cn

ssh user@host 'uptime'
来源：http://ggf.cqqwz.cn

[R58] 下载文件
来源：http://ypv.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cyx.bjfxy.top

[R59] 发 POST JSON
来源：http://qoc.tanke756.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://aev.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://wrt.jinqigufen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zgm.meibo888.top

[R61] 磁盘占用
来源：http://gzd.guowangkeji.top

df -h;  du -sh *
来源：http://gbz.yj202588.top

[R62] 找最占空间的文件
来源：http://qfj.yfazqb.com

du -ah . | sort -rh | head -10
来源：http://mdl.52xcode.cn

[R63] 内存与进程
来源：http://fkw.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://tko.ywan-chungtsiang.top

[R64] 结束进程
来源：http://mez.ppjwa.cn

kill -9 $(pgrep -f app.py)
来源：http://reu.daria6918.cn

[R65] 查看端口占用
来源：http://xlc.hongshengwenyu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hhv.fanxiaobao.xyz

[R66] 定时任务
来源：http://oho.daria6918.cn

crontab -e;  crontab -l
来源：http://ugh.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://kpk.xziqi.cn

openssl rand -hex 16
来源：http://qgv.jlsjyb.cn

[R68] 计算文件校验值
来源：http://lqb.zhongyouzk.top

sha256sum a.txt;  md5sum a.txt
来源：http://koq.wangdashe.top

[R69] 生成随机密码
来源：http://rpi.kuanghao11.cn

head -c 16 /dev/urandom | base64
来源：http://oeq.birdmap.top

[R70] 时间戳与互转
来源：http://uce.cucudq.cn

date +%s;  date -d @1700000000
来源：http://blw.guowangkeji.top

[R71] 日期格式化
来源：http://hzo.hongshengwenyu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://njh.hnqzz.top

[R72] 等待端口就绪
来源：http://edc.snrcjt.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://npn.tarul.cn

[R73] 分割大日志
来源：http://ccb.bbcook.cn

split -l 1000 big.log part_
来源：http://ftk.hnxiangtu.top

[R74] 批量重命名
来源：http://ykx.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gif.sufxvd.cn

[R75] 导出环境变量
来源：http://qus.sweek.top

export PATH="$HOME/bin:$PATH"
来源：http://ubl.zhijiandao.cn

[R76] 使用临时文件
来源：http://xen.cqqwz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bzf.fzhhl.top

[R77] 读取用户输入
来源：http://nqk.nwbrower.top

read -rp "请输入: " ans
来源：http://yep.cashguo.top

[R78] 交互式菜单
来源：http://gcq.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hyt.nwbrower.top

[R79] 解析命令行选项
来源：http://pvi.kuanghao11.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xvt.daria6918.cn

[R80] 查看脚本执行耗时
来源：http://lfa.meibo888.top

time ./run.sh
来源：http://iyo.yj202588.top

================================================================================
来源：http://wuh.epnwcf.com

S. C / C++ 专题
来源：http://xkb.daria6918.cn

================================================================================
来源：http://uhv.hesvh.cn

[S01] C：Hello World
来源：http://fjq.xziqi.cn

#include <stdio.h>
来源：http://lzo.shangyingyoupin.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://urf.redwolf501.top

[S02] C：变量与格式化输出
来源：http://exc.yj20258.top

int a = 10; printf("%d\n", a);
来源：http://hdb.shuidangran.top

[S03] C：读入整数
来源：http://wvj.dianchejie.cn

int x; scanf("%d", &x);
来源：http://npb.hysaishi.cn

[S04] C：字符串复制
来源：http://aap.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://qmy.yueranfly.top

[S05] C：字符串长度
来源：http://hio.jinqigufen.top

strlen(s)
来源：http://eqp.zhixingplan.top

[S06] C：字符串比较
来源：http://jjd.zhengqikj.top

strcmp(a, b) == 0
来源：http://vbi.yanxiufei.cn

[S07] C：数组遍历求和
来源：http://emk.mhx1999.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pny.fanxiaobao.xyz

[S08] C：动态内存分配与释放
来源：http://bsb.yuxming.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hlp.yvedp.cn

[S09] C：结构体定义与初始化
来源：http://kek.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qlh.daxiang520.top

[S10] C：指针与解引用
来源：http://hbh.yueranfly.top

int *p = &a;  *p = 5;
来源：http://oik.epnwcf.com

[S11] C：逐行读文件
来源：http://zjs.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://abp.gogol.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fzk.yangfankeji.com

fclose(f);
来源：http://vlk.aibaodan.cn

[S12] C：写文件
来源：http://ynj.fanxiaobao.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zzp.wangshuangyany.cn

[S13] C：宏定义
来源：http://vue.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://inv.zhengqikj.top

[S14] C：枚举
来源：http://eju.ydjk.org.cn

enum Color { RED, GREEN, BLUE };
来源：http://rxt.xuetiantiany.cn

[S15] C：类型转换
来源：http://wju.pycfn.com

(double) a / b
来源：http://agn.andypj.xyz

[S16] C：位操作置位
来源：http://ufm.shuidangran.top

x |= (1 << 3);
来源：http://jvc.yj20258.top

[S17] C：安全拼接字符串
来源：http://tmj.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ajj.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://bqj.yvedp.cn

int main(int argc, char **argv)
来源：http://exo.svipenyu.cn

[S19] C：快速排序
来源：http://pwr.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://smn.smart0.xyz

[S20] C：二分查找
来源：http://rbf.zhixingplan.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wgv.hesvh.cn

[S21] C：字符类别判断
来源：http://rdx.iojbl.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xyx.tanke756.top

[S22] C：字符串转数字
来源：http://ltx.fehbvm.com

atoi("42");  strtod("3.14", NULL);
来源：http://cpq.fktsv.cn

[S23] C：随机数
来源：http://wzq.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ybh.chenzaomai.com

[S24] C：获取本地时间
来源：http://cyb.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ldy.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://npm.feifeiyinyue.top

memcpy(dst, src, n);
来源：http://jyq.hnxiangtu.top

[S26] C：内存清零
来源：http://iyg.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://ouc.jinqigufen.top

[S27] C：定义常量
来源：http://jxg.52xcode.cn

const double PI = 3.14159;
来源：http://bkf.xingfuxueyuan.xyz

[S28] C：静态变量
来源：http://zau.ppjwa.cn

static int counter = 0;
来源：http://lzl.316326.xyz

[S29] C：变参函数
来源：http://wnt.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oub.pengpengdd.cyou

[S30] C：头文件保护
来源：http://mda.sufxvd.cn

#ifndef X_H
来源：http://loj.hcnkem.com

#define X_H
来源：http://uyi.hnxiangtu.top

#endif
来源：http://ptz.ywan-chungtsiang.top

[S31] C++：Hello World
来源：http://dxe.birdmap.top

#include <iostream>
来源：http://rum.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://qqa.yj20258888.top

[S32] C++：字符串
来源：http://cov.0kj1m.cn

std::string s = "hi";  s += "!";
来源：http://qed.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://zne.guannengcc.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kid.sweek.top

[S34] C++：遍历 vector
来源：http://aea.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://mby.haohaochexian.top

[S35] C++：map
来源：http://fww.c1oappe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wlx.sweek.top

[S36] C++：unordered_map
来源：http://ioe.ehwqpu.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dog.chenjidiqi.icu


<!-- 参考信息 -->