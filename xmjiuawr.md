代发 wailian999

[Q61] 移动平均
来源：http://btl.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tea.nanxinkj.top

[Q62] 分组占比
来源：http://sfq.hesvh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eef.cashguo.top

[Q63] 开启事务
来源：http://jue.gaohongyu789.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tco.shanyushiyangtech.top

[Q64] 提交事务
来源：http://owg.wangdashe.top

COMMIT;
来源：http://avy.redwolf501.top

[Q65] 回滚事务
来源：http://twe.sufxvd.cn

ROLLBACK;
来源：http://jup.zhixingplan.top

[Q66] 行锁查询
来源：http://rrj.kuanghao11.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://esb.jlsjyb.cn

[Q67] 设置隔离级别
来源：http://tcx.c1oappe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://exi.xinyue.icu

[Q68] 保存点
来源：http://pyt.zhengqikj.top

SAVEPOINT sp1;
来源：http://qur.jinyuanbaomall.cn

ROLLBACK TO sp1;
来源：http://jcd.uphjek.com

[Q69] 查看执行计划
来源：http://ban.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bzp.ctjpmb.com

[Q70] 更新统计信息
来源：http://zlg.iojbl.cn

ANALYZE TABLE users;
来源：http://pza.xziqi.cn

[Q71] 查看建表语句
来源：http://dni.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lop.ydzc1.top

[Q72] 查看索引
来源：http://vid.sufxvd.cn

SHOW INDEX FROM users;
来源：http://myp.zycfv.cn

[Q73] 查看表状态
来源：http://agp.zhoulong.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://ntr.nanxuanxn.top

[Q74] 强制使用索引
来源：http://wtt.uphjek.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fzx.hfpthk.cn

[Q75] 日期格式化
来源：http://vjx.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fbc.52xcode.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vwb.havefunace.top

[Q76] 按天统计
来源：http://lmc.hesvh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sbg.jqgufenzy.top

[Q77] 时间加减
来源：http://cgw.gogol.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lpk.mhx1999.top

[Q78] 当前时间
来源：http://sgq.zhiwuduotai.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ntz.hysaishi.cn

[Q79] 字符串拼接
来源：http://jzr.hongshengwenyu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kkq.zhengqikj.top

[Q80] 字符串截取
来源：http://yux.shanyushiyangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lam.xingfuxueyuan.xyz

[Q81] 字符串替换
来源：http://obr.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uxc.hcnkem.com

[Q82] 字符长度与字节长度
来源：http://kyg.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kko.zhoulong.xyz

[Q83] 大小写转换
来源：http://qlo.quarkkingdee.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vzs.wangshuangyany.cn

[Q84] 去除首尾空格
来源：http://yer.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://wda.hnxiangtu.top

[Q85] 数值取整
来源：http://uqu.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://awe.sxryk.cn

[Q86] 读取 JSON 字段
来源：http://mfo.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bwa.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://djn.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://idn.dianchejie.cn

[Q88] 行转列（条件聚合）
来源：http://qhv.kuanghao11.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://emd.shanyushiyangtech.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fok.ehwqpu.com

[Q89] 判断表是否存在
来源：http://nfg.tian-w.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ekz.sxryk.cn

[Q90] 生成序号列
来源：http://uan.xinyue.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://get.shzxlz.cn

================================================================================
来源：http://yva.yonumen.top

R. Bash 专题
来源：http://nya.aibaodan.cn

================================================================================
来源：http://wkx.shanyushiyangkeji.top

[R01] shebang 与严格模式
来源：http://nup.jqgufenzy.top

#!/usr/bin/env bash
来源：http://vwq.xuanzx.com

set -euo pipefail
来源：http://noe.kuanghao11.cn

[R02] 变量赋值与使用
来源：http://fuk.tanke756.top

name="Tom"; echo "$name"
来源：http://wrj.svipenyu.cn

[R03] 只读变量
来源：http://odn.zdbjq.cn

readonly PI=3.14
来源：http://kun.haohaochexian.top

[R04] 位置参数
来源：http://lew.9152youxi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://owo.shuidangran.top

[R05] 参数默认值
来源：http://eyl.wangshuangyany.cn

name="${1:-default}"
来源：http://cus.yuxming.cn

[R06] 判断命令是否存在
来源：http://rsl.birdmap.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://djt.hywenlv.cn

[R07] if 判断文件
来源：http://rzk.zhaomingkeji.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kso.meibo888.top

[R08] 数值比较
来源：http://tim.sxryk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://feb.jqgufenzy.top

[R09] 字符串比较
来源：http://qhs.sweek.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xoc.fanxiaobao.xyz

[R10] 正则匹配
来源：http://ybc.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oqo.fzhhl.top

[R11] case 多分支
来源：http://grd.hongshengwenyu.top

case "$1" in
来源：http://aml.9152youxi.cn

start) echo "启动" ;;
来源：http://aut.yvedp.cn

stop)  echo "停止" ;;
来源：http://ugo.jqgufenzy.top

*)     echo "未知命令" ;;
来源：http://cib.wangdashe.top

esac
来源：http://uti.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://ydq.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://kee.epnwcf.com

[R13] for 计数循环
来源：http://rze.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://tqg.zhijiandao.cn

[R14] C 风格 for
来源：http://vpd.ydzc1.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://brt.chenjidiqi.icu

[R15] while 逐行读文件
来源：http://ozi.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wxo.gzhubu.top

[R16] until 等待条件
来源：http://cij.shanyushiyangtech.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wmf.yonumen.top

[R17] 数组定义与取值
来源：http://yrs.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://qdh.shanyushiyangtech.top

[R18] 遍历数组
来源：http://ygl.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tqi.hywenlv.cn

[R19] 数组长度
来源：http://awz.yj20258888.top

echo "${#arr[@]}"
来源：http://thl.vqdsnc.cn

[R20] 关联数组（字典）
来源：http://ozg.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fmo.yongpay.top

[R21] 字符串长度
来源：http://iis.zhiwuduotai.top

echo "${#s}"
来源：http://cfg.yfazqb.com

[R22] 截取子串
来源：http://ahp.chenlongwang.top

echo "${s:0:5}"
来源：http://iod.shzxlz.cn

[R23] 字符串替换
来源：http://gku.zhoulong.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xyy.daria6918.cn

[R24] 大小写转换
来源：http://nhd.cdnleiting.top

echo "${s^^}"; echo "${s,,}"
来源：http://zsc.fktsv.cn

[R25] 去后缀 / 去前缀
来源：http://gar.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sfg.wangdashe.top

[R26] 命令替换
来源：http://hiy.dianchejie.cn

now=$(date +%F); echo "$now"
来源：http://pjz.yuanzhike.top

[R27] 算术展开
来源：http://qkj.dianchejie.cn

echo $((1 + 2 * 3))
来源：http://otr.jqgfzy.top

[R28] 浮点运算
来源：http://tud.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://vcy.tianlin.xyz

[R29] 定义函数
来源：http://dte.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fqv.andypj.xyz

[R30] 函数返回状态码
来源：http://rqa.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://iea.feifeiyinyue.top

[R31] 局部变量
来源：http://ihx.havefunace.top

f() { local x=1; echo "$x"; }
来源：http://kxy.nanxinkj.top

[R32] 参数个数校验
来源：http://rrv.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cdh.nanxuanxn.top

[R33] 捕获错误并提示行号
来源：http://nbt.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yjs.xuetiantiany.cn

[R34] 退出时清理
来源：http://oss.zdbjq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tdh.jqgufenzy.top

[R35] 后台执行并等待
来源：http://ahj.yanxiufei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gqh.316326.xyz

[R36] 并发执行多个任务
来源：http://xhu.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zkq.yfazqb.com

[R37] 把输出赋给变量
来源：http://wkl.zhixingplan.top

files=$(ls -1)
来源：http://xgo.birdmap.top

[R38] 管道串联
来源：http://quh.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://zsj.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://tls.sufxvd.cn

cmd > out.log 2>&1
来源：http://cnk.cucudq.cn

[R40] 追加写日志
来源：http://nea.ctjpmb.com

echo "log" >> out.log
来源：http://wvq.316326.xyz

[R41] 丢弃输出
来源：http://zib.jinqigfzy.top

cmd >/dev/null 2>&1
来源：http://gmx.jiagoushi.top

[R42] 输入重定向
来源：http://qal.jinqigufen.top

wc -l < a.txt
来源：http://nqu.yj20258888.top

[R43] 按名字查找文件
来源：http://klc.xziqi.cn

find . -name "*.log" -type f
来源：http://flh.fzhhl.top

[R44] 按修改时间查找
来源：http://vol.epnwcf.com

find . -mtime -7 -type f
来源：http://mxi.zhiwuduotai.top

[R45] 批量删除
来源：http://myf.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://rvh.yongpay.top

[R46] 递归替换文件内容
来源：http://zwg.bjfxy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wol.ivvv.top

[R47] sed 单行替换
来源：http://gso.hesvh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rkl.yanxiufei.cn

[R48] awk 取指定列
来源：http://xak.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://jsc.tianlin.xyz

[R49] awk 带条件
来源：http://llz.zhaomingkeji.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gwv.birdmap.top

[R50] awk 求和
来源：http://vup.xuanzx.com

awk '{s += $2} END {print s}' a.txt
来源：http://vua.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://ehr.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://pdw.pycfn.com

[R52] 统计行数
来源：http://zuw.chenjidiqi.icu

wc -l a.txt
来源：http://cqz.zhengqikj.top

[R53] 查看文件头与实时尾
来源：http://bub.yangfankeji.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sxf.yongpay.top

[R54] 比较两个文件
来源：http://twn.wangdashe.top

diff a.txt b.txt
来源：http://ncw.hywenlv.cn

[R55] 压缩与解压
来源：http://txc.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ifj.hcnkem.com

[R56] 远程拷贝
来源：http://wzf.shzxlz.cn

scp file user@host:/path/
来源：http://toc.yueranfly.top

[R57] 远程执行命令
来源：http://nxs.guowangkeji.top

ssh user@host 'uptime'
来源：http://lvs.hywenlv.cn

[R58] 下载文件
来源：http://fhb.mhx1999.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lif.iojbl.cn

[R59] 发 POST JSON
来源：http://ghz.svipenyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yzj.snrcjt.cn

[R60] 只看 HTTP 状态码
来源：http://lom.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zay.sxryk.cn

[R61] 磁盘占用
来源：http://zeq.cucudq.cn

df -h;  du -sh *
来源：http://vmj.yfazqb.com

[R62] 找最占空间的文件
来源：http://iqt.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://bju.jianghu66.top

[R63] 内存与进程
来源：http://hqh.gotoacloud.top

free -h;  ps aux | grep nginx
来源：http://kqd.hongshengwenyu.top

[R64] 结束进程
来源：http://jbn.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://dze.sysykeji.top

[R65] 查看端口占用
来源：http://zeq.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://czn.jianghu66.top

[R66] 定时任务
来源：http://rwt.zhijiandao.cn

crontab -e;  crontab -l
来源：http://ewj.fzhhl.top

[R67] 生成随机十六进制串
来源：http://nkc.ybcxt.top

openssl rand -hex 16
来源：http://qjd.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://tqd.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://twv.tarul.cn

[R69] 生成随机密码
来源：http://vir.xinyue.icu

head -c 16 /dev/urandom | base64
来源：http://sip.xylfe.cn

[R70] 时间戳与互转
来源：http://rka.hesvh.cn

date +%s;  date -d @1700000000
来源：http://rjd.fanxiaobao.xyz

[R71] 日期格式化
来源：http://tfg.jianghu66.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sba.smart0.xyz

[R72] 等待端口就绪
来源：http://nqf.gaohongyu789.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fqu.cdnleiting.top

[R73] 分割大日志
来源：http://whp.hnxiangtu.top

split -l 1000 big.log part_
来源：http://uuz.zhoulong.xyz

[R74] 批量重命名
来源：http://wlq.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ybw.birdmap.top

[R75] 导出环境变量
来源：http://iax.yangfankeji.com

export PATH="$HOME/bin:$PATH"
来源：http://jwu.yanxiufei.cn

[R76] 使用临时文件
来源：http://wvf.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wkj.tianlin.xyz

[R77] 读取用户输入
来源：http://hhe.daria6918.cn

read -rp "请输入: " ans
来源：http://wol.xinyue.icu

[R78] 交互式菜单
来源：http://vzw.chenlongwang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wfy.c1oappe.top

[R79] 解析命令行选项
来源：http://fhn.nanxinkj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://chz.uphjek.com

[R80] 查看脚本执行耗时
来源：http://roy.cheryme.top

time ./run.sh
来源：http://saq.c1oappe.top

================================================================================
来源：http://wdz.sxryk.cn

S. C / C++ 专题
来源：http://gfp.yonumen.top

================================================================================
来源：http://kws.nwbrower.top

[S01] C：Hello World
来源：http://iie.jqgfzy.top

#include <stdio.h>
来源：http://qib.redwolf501.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qoe.0kj1m.cn

[S02] C：变量与格式化输出
来源：http://zzg.ivvv.top

int a = 10; printf("%d\n", a);
来源：http://hfh.birdmap.top

[S03] C：读入整数
来源：http://bmd.sxryk.cn

int x; scanf("%d", &x);
来源：http://bon.hysaishi.cn

[S04] C：字符串复制
来源：http://tzy.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://adt.yueranfly.top

[S05] C：字符串长度
来源：http://cjp.jianghu66.top

strlen(s)
来源：http://nhl.nanxuanxn.top

[S06] C：字符串比较
来源：http://osf.9152youxi.cn

strcmp(a, b) == 0
来源：http://uvr.epnwcf.com

[S07] C：数组遍历求和
来源：http://nbn.wangshuangyany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vyv.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://zkm.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jdx.tian-w.cn

[S09] C：结构体定义与初始化
来源：http://vet.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://prt.vqdsnc.cn

[S10] C：指针与解引用
来源：http://azl.zhiwuduotai.top

int *p = &a;  *p = 5;
来源：http://elp.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://xfi.hnqzz.top

FILE *f = fopen("a.txt", "r");
来源：http://iap.cheryme.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ofb.hammf.cn

fclose(f);
来源：http://olg.jinghuilouyu.cn

[S12] C：写文件
来源：http://utu.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ueq.guannengcc.top

[S13] C：宏定义
来源：http://rly.jqgfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ljn.ehwqpu.com

[S14] C：枚举
来源：http://pro.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://oot.xuetiantiany.cn

[S15] C：类型转换
来源：http://kgz.ppjwa.cn

(double) a / b
来源：http://uqz.cashguo.top

[S16] C：位操作置位
来源：http://ivn.yueranfly.top

x |= (1 << 3);
来源：http://khi.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://abx.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qjr.yvedp.cn

[S18] C：命令行参数
来源：http://ols.sysykeji.top

int main(int argc, char **argv)
来源：http://svz.ydzc1.top

[S19] C：快速排序
来源：http://bpk.fanxiaobao.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://hkt.fengsongda.top

[S20] C：二分查找
来源：http://jnr.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ytu.0kj1m.cn

[S21] C：字符类别判断
来源：http://bqc.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gka.yonumen.top

[S22] C：字符串转数字
来源：http://pis.fktsv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xnc.chenzaomai.com

[S23] C：随机数
来源：http://oeu.redwolf501.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vcb.fanxiaobao.xyz

[S24] C：获取本地时间
来源：http://onz.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dqt.52xcode.cn

[S25] C：内存拷贝
来源：http://nhc.zhiwuduotai.top

memcpy(dst, src, n);
来源：http://ogc.zdbjq.cn

[S26] C：内存清零
来源：http://yuy.epnwcf.com

memset(a, 0, sizeof a);
来源：http://mwi.hammf.cn

[S27] C：定义常量
来源：http://adp.hywenlv.cn

const double PI = 3.14159;
来源：http://fdk.cheryme.top

[S28] C：静态变量
来源：http://jjl.feifeiyinyue.top

static int counter = 0;
来源：http://biw.zdqjudy.top

[S29] C：变参函数
来源：http://mgf.aibaodan.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rjl.yangfankeji.com

[S30] C：头文件保护
来源：http://oal.fanxiaobao.xyz

#ifndef X_H
来源：http://dxt.birdmap.top

#define X_H
来源：http://tkk.jiagoushi.top

#endif
来源：http://ewk.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://aer.uphjek.com


<!-- 参考信息 -->