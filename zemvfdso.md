代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://etq.c1oappe.top

[Q60] 取上一行 / 下一行
来源：http://oym.yj20258888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sei.hfpthk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bcf.hcnkem.com

[Q61] 移动平均
来源：http://mvx.fzhhl.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cwc.sweek.top

[Q62] 分组占比
来源：http://cdt.bbcook.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wad.zhijiandao.cn

[Q63] 开启事务
来源：http://cqz.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qyo.kuanghao11.cn

[Q64] 提交事务
来源：http://rrm.fengsongda.top

COMMIT;
来源：http://iif.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://hlk.yongpay.top

ROLLBACK;
来源：http://pxp.redwolf501.top

[Q66] 行锁查询
来源：http://rlj.nanxuanxn.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jyn.fktsv.cn

[Q67] 设置隔离级别
来源：http://nyt.jqgufenzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lzr.ehwqpu.com

[Q68] 保存点
来源：http://pzd.sweek.top

SAVEPOINT sp1;
来源：http://osy.zdbjq.cn

ROLLBACK TO sp1;
来源：http://gyj.shangyingyoupin.top

[Q69] 查看执行计划
来源：http://tak.shanyushiyangtech.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://axf.yonumen.top

[Q70] 更新统计信息
来源：http://ydb.jqgufenzy.top

ANALYZE TABLE users;
来源：http://fbg.fktsv.cn

[Q71] 查看建表语句
来源：http://ptr.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://skn.daxiang520.top

[Q72] 查看索引
来源：http://ufc.yueranfly.top

SHOW INDEX FROM users;
来源：http://guw.vqdsnc.cn

[Q73] 查看表状态
来源：http://fwp.daxiang520.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zic.fehbvm.com

[Q74] 强制使用索引
来源：http://wco.meibo888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qrw.fktsv.cn

[Q75] 日期格式化
来源：http://psa.yongpay.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ile.kuanghao11.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ncm.nanxuanxn.top

[Q76] 按天统计
来源：http://qxw.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pjt.zhongyouzk.top

[Q77] 时间加减
来源：http://vqo.dianchejie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rlq.gotoacloud.top

[Q78] 当前时间
来源：http://tml.fehbvm.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fwg.wangshuangyany.cn

[Q79] 字符串拼接
来源：http://kzm.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rea.daria6918.cn

[Q80] 字符串截取
来源：http://fth.yj20258.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sqm.9152youxi.cn

[Q81] 字符串替换
来源：http://sjn.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cdc.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://yta.ydzc1.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mov.vehdjk.com

[Q83] 大小写转换
来源：http://ndb.ydzc1.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fts.cqqwz.cn

[Q84] 去除首尾空格
来源：http://xkc.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://vwv.xuetiantiany.cn

[Q85] 数值取整
来源：http://hzc.fktsv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vxm.uphjek.com

[Q86] 读取 JSON 字段
来源：http://cqq.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ouo.zdbjq.cn

[Q87] JSON 字段做条件
来源：http://ugv.andypj.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ehq.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://qfa.hongshengwenyu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aks.ctjpmb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://flu.feifeiyinyue.top

[Q89] 判断表是否存在
来源：http://jae.wangdashe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lmr.cashguo.top

[Q90] 生成序号列
来源：http://paa.hesvh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wzp.zhengqikj.top

================================================================================
来源：http://bxm.yanxiufei.cn

R. Bash 专题
来源：http://nak.xuanzx.com

================================================================================
来源：http://bcc.jlsjyb.cn

[R01] shebang 与严格模式
来源：http://eow.jqgfzy.top

#!/usr/bin/env bash
来源：http://zyv.zhijiandao.cn

set -euo pipefail
来源：http://dlr.jiagoushi.top

[R02] 变量赋值与使用
来源：http://rxq.nwbrower.top

name="Tom"; echo "$name"
来源：http://wnn.zhijiandao.cn

[R03] 只读变量
来源：http://mdn.jinqigufen.top

readonly PI=3.14
来源：http://qrl.yj20258.top

[R04] 位置参数
来源：http://rjf.cqqwz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://skj.xuanzx.com

[R05] 参数默认值
来源：http://jpc.aizwys.cn

name="${1:-default}"
来源：http://evp.sxryk.cn

[R06] 判断命令是否存在
来源：http://zkc.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gya.andypj.xyz

[R07] if 判断文件
来源：http://wpn.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wia.cheryme.top

[R08] 数值比较
来源：http://qct.zdqjudy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://xdr.cucudq.cn

[R09] 字符串比较
来源：http://wez.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wrx.sweek.top

[R10] 正则匹配
来源：http://aus.yonumen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jwf.daria6918.cn

[R11] case 多分支
来源：http://wzu.yuxming.cn

case "$1" in
来源：http://uee.cqqwz.cn

start) echo "启动" ;;
来源：http://nzz.sweek.top

stop)  echo "停止" ;;
来源：http://ekk.fzhhl.top

*)     echo "未知命令" ;;
来源：http://rbf.shuidangran.top

esac
来源：http://sye.haohaochexian.top

[R12] for 遍历文件
来源：http://gva.9152youxi.cn

for f in *.txt; do echo "$f"; done
来源：http://hht.smart0.xyz

[R13] for 计数循环
来源：http://fun.jinghuilouyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://ltm.birdmap.top

[R14] C 风格 for
来源：http://gfk.guowangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ien.tarul.cn

[R15] while 逐行读文件
来源：http://tzv.zhengqikj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uag.jinghuilouyu.cn

[R16] until 等待条件
来源：http://qju.fengsongda.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jyu.jlsjyb.cn

[R17] 数组定义与取值
来源：http://wul.ivvv.top

arr=(a b c); echo "${arr[0]}"
来源：http://dha.zhongyouzk.top

[R18] 遍历数组
来源：http://zpp.shanyushiyangtech.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tnu.yueranfly.top

[R19] 数组长度
来源：http://kax.jiagoushi.top

echo "${#arr[@]}"
来源：http://iwj.andypj.xyz

[R20] 关联数组（字典）
来源：http://wmc.zhengqikj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bnw.cqqwz.cn

[R21] 字符串长度
来源：http://mzz.yonumen.top

echo "${#s}"
来源：http://qwp.feifeiyinyue.top

[R22] 截取子串
来源：http://fnl.birdmap.top

echo "${s:0:5}"
来源：http://wri.redwolf501.top

[R23] 字符串替换
来源：http://doi.jiagoushi.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jfn.shanyushiyangtech.top

[R24] 大小写转换
来源：http://qjn.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://hyf.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://arn.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kha.chenzaomai.com

[R26] 命令替换
来源：http://gqm.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://bkg.316326.xyz

[R27] 算术展开
来源：http://dcm.xylfe.cn

echo $((1 + 2 * 3))
来源：http://sht.aizwys.cn

[R28] 浮点运算
来源：http://oaj.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://gmu.nanxinkj.top

[R29] 定义函数
来源：http://yjz.nanxinkj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://njb.guannengcc.top

[R30] 函数返回状态码
来源：http://soe.yanxiufei.cn

f() { return 0; }; f || echo "失败了"
来源：http://ioa.zhixingplan.top

[R31] 局部变量
来源：http://wne.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://vnu.yfazqb.com

[R32] 参数个数校验
来源：http://cbk.yuanzhike.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ltg.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://jqk.ctjpmb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wqb.hcnkem.com

[R34] 退出时清理
来源：http://txx.zdqjudy.top

trap 'rm -f "$tmp"' EXIT
来源：http://czu.redwolf501.top

[R35] 后台执行并等待
来源：http://rye.svipenyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gki.fengsongda.top

[R36] 并发执行多个任务
来源：http://cmh.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bwh.jinqigufen.top

[R37] 把输出赋给变量
来源：http://hwu.ywan-chungtsiang.top

files=$(ls -1)
来源：http://gpx.smart0.xyz

[R38] 管道串联
来源：http://czu.jiagoushi.top

cat a.txt | grep -i error | wc -l
来源：http://doi.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://iut.316326.xyz

cmd > out.log 2>&1
来源：http://snf.fktsv.cn

[R40] 追加写日志
来源：http://pum.jinqigufen.top

echo "log" >> out.log
来源：http://hzk.ppjwa.cn

[R41] 丢弃输出
来源：http://pkc.hfpthk.cn

cmd >/dev/null 2>&1
来源：http://bqo.ydzc1.top

[R42] 输入重定向
来源：http://duc.zhixingplan.top

wc -l < a.txt
来源：http://gor.yj20258.top

[R43] 按名字查找文件
来源：http://arg.chenzaomai.com

find . -name "*.log" -type f
来源：http://aup.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://ysm.yuanzhike.top

find . -mtime -7 -type f
来源：http://suf.316326.xyz

[R45] 批量删除
来源：http://tzj.zhoulong.xyz

find . -name "*.tmp" -delete
来源：http://dav.hywenlv.cn

[R46] 递归替换文件内容
来源：http://jwu.ybcxt.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vzh.uphjek.com

[R47] sed 单行替换
来源：http://lpo.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://ckw.zhiwuduotai.top

[R48] awk 取指定列
来源：http://mav.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://yal.xziqi.cn

[R49] awk 带条件
来源：http://cja.pengpengdd.cyou

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ort.jianghu66.top

[R50] awk 求和
来源：http://orm.gaohongyu789.top

awk '{s += $2} END {print s}' a.txt
来源：http://fcz.kuanghao11.cn

[R51] 排序去重取前几
来源：http://ski.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dfm.daria6918.cn

[R52] 统计行数
来源：http://jpj.316326.xyz

wc -l a.txt
来源：http://phg.chenjidiqi.icu

[R53] 查看文件头与实时尾
来源：http://vhm.cucudq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ncx.hnxiangtu.top

[R54] 比较两个文件
来源：http://yqk.9152youxi.cn

diff a.txt b.txt
来源：http://aqy.vehdjk.com

[R55] 压缩与解压
来源：http://mlo.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ltp.gogol.net.cn

[R56] 远程拷贝
来源：http://yrh.zhongyouzk.top

scp file user@host:/path/
来源：http://atz.aibaodan.cn

[R57] 远程执行命令
来源：http://lbn.cqqwz.cn

ssh user@host 'uptime'
来源：http://mld.zhijiandao.cn

[R58] 下载文件
来源：http://rbt.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qfq.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://fdk.birdmap.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uat.xuanzx.com

[R60] 只看 HTTP 状态码
来源：http://tho.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://otr.bjfxy.top

[R61] 磁盘占用
来源：http://sel.gzhubu.top

df -h;  du -sh *
来源：http://woc.hnxiangtu.top

[R62] 找最占空间的文件
来源：http://mfv.sweek.top

du -ah . | sort -rh | head -10
来源：http://fhl.svipenyu.cn

[R63] 内存与进程
来源：http://nqn.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://bsv.chenzaomai.com

[R64] 结束进程
来源：http://ohj.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://eni.tianlin.xyz

[R65] 查看端口占用
来源：http://vsr.daria6918.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wqb.smart0.xyz

[R66] 定时任务
来源：http://slo.hnqzz.top

crontab -e;  crontab -l
来源：http://fbb.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://kuf.pycfn.com

openssl rand -hex 16
来源：http://mvx.hesvh.cn

[R68] 计算文件校验值
来源：http://sci.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://cpw.cheryme.top

[R69] 生成随机密码
来源：http://szx.aibaodan.cn

head -c 16 /dev/urandom | base64
来源：http://ecr.yonumen.top

[R70] 时间戳与互转
来源：http://gvj.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://chv.zycfv.cn

[R71] 日期格式化
来源：http://rin.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://asv.vehdjk.com

[R72] 等待端口就绪
来源：http://syt.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sxo.yj20258888.top

[R73] 分割大日志
来源：http://yas.zhengqikj.top

split -l 1000 big.log part_
来源：http://dhw.yuanzhike.top

[R74] 批量重命名
来源：http://fvq.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zyk.tian-w.cn

[R75] 导出环境变量
来源：http://xza.dashuyun.cn

export PATH="$HOME/bin:$PATH"
来源：http://rfp.hcnkem.com

[R76] 使用临时文件
来源：http://rsf.shanyushiyangtech.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://evw.meibo888.top

[R77] 读取用户输入
来源：http://iqh.jyoumei.cn

read -rp "请输入: " ans
来源：http://gnv.316326.xyz

[R78] 交互式菜单
来源：http://spu.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xak.tarul.cn

[R79] 解析命令行选项
来源：http://gvj.ybcxt.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kfz.yj20258.top

[R80] 查看脚本执行耗时
来源：http://cgr.nanxinkj.top

time ./run.sh
来源：http://jrq.hfpthk.cn

================================================================================
来源：http://dvk.hcnkem.com

S. C / C++ 专题
来源：http://pmb.52xcode.cn

================================================================================
来源：http://gvl.ppjwa.cn

[S01] C：Hello World
来源：http://dxn.fengsongda.top

#include <stdio.h>
来源：http://dzi.hnxiangtu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://imw.sjlbkw.cn

[S02] C：变量与格式化输出
来源：http://djp.fzhhl.top

int a = 10; printf("%d\n", a);
来源：http://dcp.hywenlv.cn

[S03] C：读入整数
来源：http://yia.hongshengwenyu.top

int x; scanf("%d", &x);
来源：http://mrf.daxiang520.top

[S04] C：字符串复制
来源：http://sav.fanxiaobao.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://rbf.yvedp.cn

[S05] C：字符串长度
来源：http://enp.epnwcf.com

strlen(s)
来源：http://gre.meibo888.top

[S06] C：字符串比较
来源：http://dal.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://xmq.yongpay.top

[S07] C：数组遍历求和
来源：http://fpi.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ocr.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://btg.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ltu.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://rbh.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tll.yj20258888.top

[S10] C：指针与解引用
来源：http://dfr.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://bfz.xuanzx.com

[S11] C：逐行读文件
来源：http://ryi.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://xdr.guowangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rzy.snrcjt.cn

fclose(f);
来源：http://obv.yongpay.top

[S12] C：写文件
来源：http://lyf.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fhh.daxiang520.top

[S13] C：宏定义
来源：http://fai.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qmr.xziqi.cn

[S14] C：枚举
来源：http://npr.sysykeji.top

enum Color { RED, GREEN, BLUE };
来源：http://rbj.zhoulong.xyz

[S15] C：类型转换
来源：http://qcx.316326.xyz

(double) a / b
来源：http://uir.svipenyu.cn

[S16] C：位操作置位
来源：http://gop.hongshengwenyu.top

x |= (1 << 3);
来源：http://tke.tarul.cn

[S17] C：安全拼接字符串
来源：http://gny.zhijiandao.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bwf.yuanzhike.top

[S18] C：命令行参数
来源：http://kre.hesvh.cn

int main(int argc, char **argv)
来源：http://rah.nanxuanxn.top

[S19] C：快速排序
来源：http://fhk.gaohongyu789.top

qsort(a, n, sizeof(int), cmp);
来源：http://aet.yj20258888.top

[S20] C：二分查找
来源：http://uwn.fktsv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nox.52xcode.cn

[S21] C：字符类别判断
来源：http://yxq.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ljt.hnxiangtu.top

[S22] C：字符串转数字
来源：http://vba.dashuyun.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rmb.ywan-chungtsiang.top

[S23] C：随机数
来源：http://hzf.pycfn.com

srand(time(NULL));  int r = rand() % 100;
来源：http://wjg.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://zlh.ppjwa.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sob.tian-w.cn

[S25] C：内存拷贝
来源：http://zfh.tanke756.top

memcpy(dst, src, n);
来源：http://kyw.wangdashe.top

[S26] C：内存清零
来源：http://bvk.nwbrower.top

memset(a, 0, sizeof a);
来源：http://tte.ehwqpu.com

[S27] C：定义常量
来源：http://qgk.sjlbkw.cn

const double PI = 3.14159;
来源：http://ofd.jlsjyb.cn

[S28] C：静态变量
来源：http://nfk.yongpay.top

static int counter = 0;
来源：http://dvq.andypj.xyz

[S29] C：变参函数
来源：http://zbk.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ial.tanke756.top

[S30] C：头文件保护
来源：http://sre.vqdsnc.cn


<!-- 参考信息 -->