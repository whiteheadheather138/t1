代发 wailian999

[Q63] 开启事务
来源：http://asm.guowangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tus.hywenlv.cn

[Q64] 提交事务
来源：http://xlg.hammf.cn

COMMIT;
来源：http://ruf.nanxuanxn.top

[Q65] 回滚事务
来源：http://mgj.yueranfly.top

ROLLBACK;
来源：http://cit.redwolf501.top

[Q66] 行锁查询
来源：http://bqq.kuanghao11.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zxi.epnwcf.com

[Q67] 设置隔离级别
来源：http://pyo.jyoumei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://crp.cucudq.cn

[Q68] 保存点
来源：http://kic.sjlbkw.cn

SAVEPOINT sp1;
来源：http://gvk.jqgfzy.top

ROLLBACK TO sp1;
来源：http://ylk.epnwcf.com

[Q69] 查看执行计划
来源：http://coi.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ynj.zhoulong.xyz

[Q70] 更新统计信息
来源：http://lpd.birdmap.top

ANALYZE TABLE users;
来源：http://umq.zhengqikj.top

[Q71] 查看建表语句
来源：http://qti.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vfe.shanyushiyangkeji.top

[Q72] 查看索引
来源：http://tlq.hnqzz.top

SHOW INDEX FROM users;
来源：http://oqp.316326.xyz

[Q73] 查看表状态
来源：http://uej.chenjidiqi.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://zco.nanxuanxn.top

[Q74] 强制使用索引
来源：http://bzr.quarkkingdee.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pxq.0kj1m.cn

[Q75] 日期格式化
来源：http://zqy.redwolf501.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yzd.fzhhl.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://loh.hywenlv.cn

[Q76] 按天统计
来源：http://rfl.nwbrower.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kxj.vehdjk.com

[Q77] 时间加减
来源：http://rbh.ybcxt.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ijc.ivvv.top

[Q78] 当前时间
来源：http://htl.vehdjk.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fbt.bjfxy.top

[Q79] 字符串拼接
来源：http://fpm.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jui.yueranfly.top

[Q80] 字符串截取
来源：http://mtf.sjlbkw.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nwp.fengsongda.top

[Q81] 字符串替换
来源：http://nku.pycfn.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mlp.smart0.xyz

[Q82] 字符长度与字节长度
来源：http://xgu.yanxiufei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dtd.tarul.cn

[Q83] 大小写转换
来源：http://vxv.yueranfly.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jci.vehdjk.com

[Q84] 去除首尾空格
来源：http://rxq.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://hhh.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://opl.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vvu.jlsjyb.cn

[Q86] 读取 JSON 字段
来源：http://tde.zhiwuduotai.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aed.0kj1m.cn

[Q87] JSON 字段做条件
来源：http://ggb.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qrs.jianghu66.top

[Q88] 行转列（条件聚合）
来源：http://ygp.jinqigfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qmp.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ujb.cashguo.top

[Q89] 判断表是否存在
来源：http://ojz.zhijiandao.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://akt.ydjk.org.cn

[Q90] 生成序号列
来源：http://rpy.sxryk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ncd.xziqi.cn

================================================================================
来源：http://lqu.jianghu66.top

R. Bash 专题
来源：http://esd.yj202588.top

================================================================================
来源：http://way.gzhubu.top

[R01] shebang 与严格模式
来源：http://ups.zhengqikj.top

#!/usr/bin/env bash
来源：http://nef.wangshuangyany.cn

set -euo pipefail
来源：http://yhe.bbcook.cn

[R02] 变量赋值与使用
来源：http://tmo.yfazqb.com

name="Tom"; echo "$name"
来源：http://hbb.fktsv.cn

[R03] 只读变量
来源：http://eva.xziqi.cn

readonly PI=3.14
来源：http://wki.jlsjyb.cn

[R04] 位置参数
来源：http://iqm.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mgd.shangyingyoupin.top

[R05] 参数默认值
来源：http://ika.bbcook.cn

name="${1:-default}"
来源：http://nkn.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://dwd.pengpengdd.cyou

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kll.mhx1999.top

[R07] if 判断文件
来源：http://hng.meibo888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jtc.sxryk.cn

[R08] 数值比较
来源：http://rdg.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cxi.sxryk.cn

[R09] 字符串比较
来源：http://nrg.jyoumei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://huo.wangdashe.top

[R10] 正则匹配
来源：http://vcc.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yph.xziqi.cn

[R11] case 多分支
来源：http://auc.redwolf501.top

case "$1" in
来源：http://mlj.hongshengwenyu.top

start) echo "启动" ;;
来源：http://odw.guowangkeji.top

stop)  echo "停止" ;;
来源：http://exu.yuanzhike.top

*)     echo "未知命令" ;;
来源：http://ooj.yuanzhike.top

esac
来源：http://ofj.hnqzz.top

[R12] for 遍历文件
来源：http://hvv.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://qek.zycfv.cn

[R13] for 计数循环
来源：http://efg.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://gvw.fktsv.cn

[R14] C 风格 for
来源：http://buh.xuanzx.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wdf.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://rkw.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dqw.smart0.xyz

[R16] until 等待条件
来源：http://mpt.tanke756.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fcj.mhx1999.top

[R17] 数组定义与取值
来源：http://zvl.52xcode.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rkx.zhixingplan.top

[R18] 遍历数组
来源：http://yel.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yhj.ydjk.org.cn

[R19] 数组长度
来源：http://him.yfazqb.com

echo "${#arr[@]}"
来源：http://gmc.nanxinkj.top

[R20] 关联数组（字典）
来源：http://mxc.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yhm.cqqwz.cn

[R21] 字符串长度
来源：http://tqj.aizwys.cn

echo "${#s}"
来源：http://how.vehdjk.com

[R22] 截取子串
来源：http://bep.52xcode.cn

echo "${s:0:5}"
来源：http://ogy.yuxming.cn

[R23] 字符串替换
来源：http://zwu.hnqzz.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jzh.yangfankeji.com

[R24] 大小写转换
来源：http://rqy.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://pjz.epnwcf.com

[R25] 去后缀 / 去前缀
来源：http://jkv.shangyingyoupin.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fox.mhx1999.top

[R26] 命令替换
来源：http://xrx.hnqzz.top

now=$(date +%F); echo "$now"
来源：http://cnq.sysykeji.top

[R27] 算术展开
来源：http://ysp.fengsongda.top

echo $((1 + 2 * 3))
来源：http://pvp.epnwcf.com

[R28] 浮点运算
来源：http://byp.hnqzz.top

echo "scale=2; 10/3" | bc
来源：http://bwf.sufxvd.cn

[R29] 定义函数
来源：http://uae.dianchejie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kpe.vehdjk.com

[R30] 函数返回状态码
来源：http://tan.ctjpmb.com

f() { return 0; }; f || echo "失败了"
来源：http://gjc.hysaishi.cn

[R31] 局部变量
来源：http://gyp.guannengcc.top

f() { local x=1; echo "$x"; }
来源：http://ify.guannengcc.top

[R32] 参数个数校验
来源：http://bor.hywenlv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bjf.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://ewh.ybcxt.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hel.tianlin.xyz

[R34] 退出时清理
来源：http://gxo.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://uhd.0kj1m.cn

[R35] 后台执行并等待
来源：http://mey.guannengcc.top

sleep 5 & pid=$!; wait "$pid"
来源：http://omf.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://mvf.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://psd.nanxuanxn.top

[R37] 把输出赋给变量
来源：http://swl.zycfv.cn

files=$(ls -1)
来源：http://cer.fzhhl.top

[R38] 管道串联
来源：http://iib.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://szx.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://sod.zdqjudy.top

cmd > out.log 2>&1
来源：http://kil.hammf.cn

[R40] 追加写日志
来源：http://hhi.gotoacloud.top

echo "log" >> out.log
来源：http://dni.jinyuanbaomall.cn

[R41] 丢弃输出
来源：http://zwi.jlsjyb.cn

cmd >/dev/null 2>&1
来源：http://dhr.iojbl.cn

[R42] 输入重定向
来源：http://hlg.wangshuangyany.cn

wc -l < a.txt
来源：http://qhk.vehdjk.com

[R43] 按名字查找文件
来源：http://hjb.aibaodan.cn

find . -name "*.log" -type f
来源：http://nvf.zdqjudy.top

[R44] 按修改时间查找
来源：http://haz.redwolf501.top

find . -mtime -7 -type f
来源：http://kge.snrcjt.cn

[R45] 批量删除
来源：http://cjk.fktsv.cn

find . -name "*.tmp" -delete
来源：http://uax.zdqjudy.top

[R46] 递归替换文件内容
来源：http://ldy.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kkr.xuanzx.com

[R47] sed 单行替换
来源：http://gxi.shzxlz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lik.ctjpmb.com

[R48] awk 取指定列
来源：http://lnc.aizwys.cn

awk '{print $1, $3}' a.txt
来源：http://wto.cucudq.cn

[R49] awk 带条件
来源：http://qzf.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pjq.zhiwuduotai.top

[R50] awk 求和
来源：http://psu.ydzc1.top

awk '{s += $2} END {print s}' a.txt
来源：http://vzu.hesvh.cn

[R51] 排序去重取前几
来源：http://rum.fzhhl.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cwi.9152youxi.cn

[R52] 统计行数
来源：http://jqo.tanke756.top

wc -l a.txt
来源：http://qms.bbcook.cn

[R53] 查看文件头与实时尾
来源：http://nbp.hysaishi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dti.xylfe.cn

[R54] 比较两个文件
来源：http://qoy.hnqzz.top

diff a.txt b.txt
来源：http://wqe.haohaochexian.top

[R55] 压缩与解压
来源：http://jjn.ydjk.org.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xag.jinqigfzy.top

[R56] 远程拷贝
来源：http://xfo.gaohongyu789.top

scp file user@host:/path/
来源：http://nxc.jiagoushi.top

[R57] 远程执行命令
来源：http://wst.guannengcc.top

ssh user@host 'uptime'
来源：http://ahy.jinqigfzy.top

[R58] 下载文件
来源：http://bfn.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nbc.zycfv.cn

[R59] 发 POST JSON
来源：http://qtm.52xcode.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vor.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://xke.ywan-chungtsiang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qek.shzxlz.cn

[R61] 磁盘占用
来源：http://klc.zhongyouzk.top

df -h;  du -sh *
来源：http://bil.hnxiangtu.top

[R62] 找最占空间的文件
来源：http://igh.shuidangran.top

du -ah . | sort -rh | head -10
来源：http://abg.yanxiufei.cn

[R63] 内存与进程
来源：http://tsv.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://yyh.xuetiantiany.cn

[R64] 结束进程
来源：http://nqu.316326.xyz

kill -9 $(pgrep -f app.py)
来源：http://pkg.pycfn.com

[R65] 查看端口占用
来源：http://foq.hongshengwenyu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gmp.zhijiandao.cn

[R66] 定时任务
来源：http://afi.uphjek.com

crontab -e;  crontab -l
来源：http://kyo.redwolf501.top

[R67] 生成随机十六进制串
来源：http://hoe.daria6918.cn

openssl rand -hex 16
来源：http://hnz.pycfn.com

[R68] 计算文件校验值
来源：http://iag.ydjk.org.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kfw.zhixingplan.top

[R69] 生成随机密码
来源：http://dav.andypj.xyz

head -c 16 /dev/urandom | base64
来源：http://ryd.52xcode.cn

[R70] 时间戳与互转
来源：http://hcv.shuidangran.top

date +%s;  date -d @1700000000
来源：http://awb.pycfn.com

[R71] 日期格式化
来源：http://mqs.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nme.sxryk.cn

[R72] 等待端口就绪
来源：http://swh.aibaodan.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zpd.havefunace.top

[R73] 分割大日志
来源：http://ycy.fzhhl.top

split -l 1000 big.log part_
来源：http://whm.jianghu66.top

[R74] 批量重命名
来源：http://gbu.sjlbkw.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gvo.birdmap.top

[R75] 导出环境变量
来源：http://eho.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://why.hnqzz.top

[R76] 使用临时文件
来源：http://rhn.yueranfly.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vau.dashuyun.cn

[R77] 读取用户输入
来源：http://yxx.hysaishi.cn

read -rp "请输入: " ans
来源：http://qwb.ctjpmb.com

[R78] 交互式菜单
来源：http://dkm.mhx1999.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uhi.sufxvd.cn

[R79] 解析命令行选项
来源：http://vre.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ubq.pycfn.com

[R80] 查看脚本执行耗时
来源：http://uiz.vqdsnc.cn

time ./run.sh
来源：http://abg.fktsv.cn

================================================================================
来源：http://kxz.yuxming.cn

S. C / C++ 专题
来源：http://kqp.shanyushiyangkeji.top

================================================================================
来源：http://dsm.hnxiangtu.top

[S01] C：Hello World
来源：http://yuh.hfpthk.cn

#include <stdio.h>
来源：http://aor.zhixingplan.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://uug.smart0.xyz

[S02] C：变量与格式化输出
来源：http://upb.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://vun.zdbjq.cn

[S03] C：读入整数
来源：http://sep.meibo888.top

int x; scanf("%d", &x);
来源：http://ryh.gaohongyu789.top

[S04] C：字符串复制
来源：http://njm.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://lvk.hongshengwenyu.top

[S05] C：字符串长度
来源：http://rfj.hongshengwenyu.top

strlen(s)
来源：http://dsu.tanke756.top

[S06] C：字符串比较
来源：http://zpx.jqgufenzy.top

strcmp(a, b) == 0
来源：http://prt.zycfv.cn

[S07] C：数组遍历求和
来源：http://uml.316326.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vwu.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://ots.hnqzz.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eid.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://ipm.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sum.aizwys.cn

[S10] C：指针与解引用
来源：http://jbq.cheryme.top

int *p = &a;  *p = 5;
来源：http://ozz.tian-w.cn

[S11] C：逐行读文件
来源：http://ikt.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://mpi.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oyr.cqqwz.cn

fclose(f);
来源：http://hfj.zdbjq.cn

[S12] C：写文件
来源：http://sqp.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iwv.yfazqb.com

[S13] C：宏定义
来源：http://jvp.yuxming.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tyx.yuxming.cn

[S14] C：枚举
来源：http://amb.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://gqb.yueranfly.top

[S15] C：类型转换
来源：http://ogv.jinqigfzy.top

(double) a / b
来源：http://whm.uphjek.com

[S16] C：位操作置位
来源：http://gde.gogol.net.cn

x |= (1 << 3);
来源：http://ifk.dianchejie.cn

[S17] C：安全拼接字符串
来源：http://dsj.chenjidiqi.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cxj.haohaochexian.top

[S18] C：命令行参数
来源：http://twz.9152youxi.cn

int main(int argc, char **argv)
来源：http://eyq.nwbrower.top

[S19] C：快速排序
来源：http://kyr.vqdsnc.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qxz.bjfxy.top

[S20] C：二分查找
来源：http://tcm.xziqi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://krn.zycfv.cn

[S21] C：字符类别判断
来源：http://tfm.jqgufenzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qhb.tian-w.cn

[S22] C：字符串转数字
来源：http://rjm.jqgfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://sal.havefunace.top

[S23] C：随机数
来源：http://cng.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ljj.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://zlg.0kj1m.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fwe.feifeiyinyue.top

[S25] C：内存拷贝
来源：http://bsz.yj20258.top

memcpy(dst, src, n);
来源：http://zdw.ctjpmb.com

[S26] C：内存清零
来源：http://jve.xuanzx.com

memset(a, 0, sizeof a);
来源：http://jxg.yuxming.cn

[S27] C：定义常量
来源：http://jzi.xingfuxueyuan.xyz

const double PI = 3.14159;
来源：http://lju.andypj.xyz

[S28] C：静态变量
来源：http://evx.uphjek.com

static int counter = 0;
来源：http://pgf.jlsjyb.cn

[S29] C：变参函数
来源：http://nzz.52xcode.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nkz.shuidangran.top

[S30] C：头文件保护
来源：http://dqx.ywan-chungtsiang.top

#ifndef X_H
来源：http://rvd.ppjwa.cn

#define X_H
来源：http://ukz.meibo888.top

#endif
来源：http://gzt.c1oappe.top

[S31] C++：Hello World
来源：http://hio.yuanzhike.top

#include <iostream>
来源：http://lqs.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://cku.aizwys.cn

[S32] C++：字符串
来源：http://thf.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://uon.fengsongda.top


<!-- 参考信息 -->