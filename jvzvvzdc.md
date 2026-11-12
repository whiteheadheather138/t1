代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ahu.ydzc1.top

[Q60] 取上一行 / 下一行
来源：http://nep.yj20258888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://far.hysaishi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rjg.tian-w.cn

[Q61] 移动平均
来源：http://ifc.fanxiaobao.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jrb.kuanghao11.cn

[Q62] 分组占比
来源：http://loa.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jbh.yj202588.top

[Q63] 开启事务
来源：http://yai.daxiang520.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xmi.jianghu66.top

[Q64] 提交事务
来源：http://dqg.zdqjudy.top

COMMIT;
来源：http://tfk.cqqwz.cn

[Q65] 回滚事务
来源：http://qsh.316326.xyz

ROLLBACK;
来源：http://wbt.bjfxy.top

[Q66] 行锁查询
来源：http://nye.cashguo.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oma.hywenlv.cn

[Q67] 设置隔离级别
来源：http://kby.ydzc1.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ish.tanke756.top

[Q68] 保存点
来源：http://urj.pengpengdd.cyou

SAVEPOINT sp1;
来源：http://eld.316326.xyz

ROLLBACK TO sp1;
来源：http://fcq.hongshengwenyu.top

[Q69] 查看执行计划
来源：http://uxl.hnqzz.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://srd.yonumen.top

[Q70] 更新统计信息
来源：http://faj.tarul.cn

ANALYZE TABLE users;
来源：http://mpt.chenzaomai.com

[Q71] 查看建表语句
来源：http://mbj.zhiwuduotai.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ivz.jiagoushi.top

[Q72] 查看索引
来源：http://cfc.fengsongda.top

SHOW INDEX FROM users;
来源：http://vaq.gzhubu.top

[Q73] 查看表状态
来源：http://ibj.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://iuc.ywan-chungtsiang.top

[Q74] 强制使用索引
来源：http://cdq.gzhubu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hnx.aizwys.cn

[Q75] 日期格式化
来源：http://sxb.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://amy.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hax.daxiang520.top

[Q76] 按天统计
来源：http://dut.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://buo.iojbl.cn

[Q77] 时间加减
来源：http://iyt.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yrx.0kj1m.cn

[Q78] 当前时间
来源：http://xue.vehdjk.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wyi.chenzaomai.com

[Q79] 字符串拼接
来源：http://wow.xziqi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zip.hesvh.cn

[Q80] 字符串截取
来源：http://kkk.sjlbkw.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hgj.cucudq.cn

[Q81] 字符串替换
来源：http://hxs.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kal.guowangkeji.top

[Q82] 字符长度与字节长度
来源：http://ccq.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qiw.zhiwuduotai.top

[Q83] 大小写转换
来源：http://uci.tanke756.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uqe.smart0.xyz

[Q84] 去除首尾空格
来源：http://efm.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://lgu.fengsongda.top

[Q85] 数值取整
来源：http://nku.nanxuanxn.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tpo.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://xre.hesvh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://quh.bjfxy.top

[Q87] JSON 字段做条件
来源：http://cfs.tian-w.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xqm.zycfv.cn

[Q88] 行转列（条件聚合）
来源：http://rxs.fanxiaobao.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lxp.ybcxt.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xhb.zdbjq.cn

[Q89] 判断表是否存在
来源：http://yhx.mhx1999.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xvg.nwbrower.top

[Q90] 生成序号列
来源：http://hym.guowangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://arf.c1oappe.top

================================================================================
来源：http://dnt.316326.xyz

R. Bash 专题
来源：http://bix.chenlongwang.top

================================================================================
来源：http://lor.yfazqb.com

[R01] shebang 与严格模式
来源：http://ive.dianchejie.cn

#!/usr/bin/env bash
来源：http://zwb.yonumen.top

set -euo pipefail
来源：http://kzx.zdbjq.cn

[R02] 变量赋值与使用
来源：http://rmg.ybcxt.top

name="Tom"; echo "$name"
来源：http://ygq.wangdashe.top

[R03] 只读变量
来源：http://rrk.sweek.top

readonly PI=3.14
来源：http://nly.shanyushiyangkeji.top

[R04] 位置参数
来源：http://nvh.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ljd.jianghu66.top

[R05] 参数默认值
来源：http://vvy.hammf.cn

name="${1:-default}"
来源：http://jqm.ppjwa.cn

[R06] 判断命令是否存在
来源：http://yvr.havefunace.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hil.aibaodan.cn

[R07] if 判断文件
来源：http://itt.andypj.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kat.aizwys.cn

[R08] 数值比较
来源：http://yrq.yueranfly.top

if (( a > b )); then echo "a 更大"; fi
来源：http://kzd.xylfe.cn

[R09] 字符串比较
来源：http://noi.yuxming.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://psg.jinqigufen.top

[R10] 正则匹配
来源：http://aft.gaohongyu789.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aus.hammf.cn

[R11] case 多分支
来源：http://tag.jinqigfzy.top

case "$1" in
来源：http://xsl.yueranfly.top

start) echo "启动" ;;
来源：http://iul.xuanzx.com

stop)  echo "停止" ;;
来源：http://psy.shzxlz.cn

*)     echo "未知命令" ;;
来源：http://afk.yuxming.cn

esac
来源：http://cem.snrcjt.cn

[R12] for 遍历文件
来源：http://zog.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://pxk.andypj.xyz

[R13] for 计数循环
来源：http://nce.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://mno.bjfxy.top

[R14] C 风格 for
来源：http://vxt.daxiang520.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pev.epnwcf.com

[R15] while 逐行读文件
来源：http://wlt.birdmap.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://frz.svipenyu.cn

[R16] until 等待条件
来源：http://ltz.gotoacloud.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qis.yj20258888.top

[R17] 数组定义与取值
来源：http://ttd.zhixingplan.top

arr=(a b c); echo "${arr[0]}"
来源：http://ogf.epnwcf.com

[R18] 遍历数组
来源：http://gcs.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vvb.tarul.cn

[R19] 数组长度
来源：http://rly.zhaomingkeji.xyz

echo "${#arr[@]}"
来源：http://ogr.zhongyouzk.top

[R20] 关联数组（字典）
来源：http://gdz.jyoumei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qrp.xuanzx.com

[R21] 字符串长度
来源：http://ieh.hfpthk.cn

echo "${#s}"
来源：http://iux.bbcook.cn

[R22] 截取子串
来源：http://kfa.xziqi.cn

echo "${s:0:5}"
来源：http://art.zhixingplan.top

[R23] 字符串替换
来源：http://qox.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://drl.gotoacloud.top

[R24] 大小写转换
来源：http://kgu.jinqigufen.top

echo "${s^^}"; echo "${s,,}"
来源：http://qzc.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://dio.sjlbkw.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oni.52xcode.cn

[R26] 命令替换
来源：http://ems.jianghu66.top

now=$(date +%F); echo "$now"
来源：http://ybi.fengsongda.top

[R27] 算术展开
来源：http://tky.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://fcm.316326.xyz

[R28] 浮点运算
来源：http://ayp.andypj.xyz

echo "scale=2; 10/3" | bc
来源：http://zcu.ybcxt.top

[R29] 定义函数
来源：http://ohw.dianchejie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://max.vehdjk.com

[R30] 函数返回状态码
来源：http://gzs.ydzc1.top

f() { return 0; }; f || echo "失败了"
来源：http://dsg.ybcxt.top

[R31] 局部变量
来源：http://kry.zhengqikj.top

f() { local x=1; echo "$x"; }
来源：http://bae.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://uxh.yanxiufei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ung.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://ruu.shzxlz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nkt.jqgfzy.top

[R34] 退出时清理
来源：http://obq.hfpthk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jbn.uphjek.com

[R35] 后台执行并等待
来源：http://qwd.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pwt.jinqigufen.top

[R36] 并发执行多个任务
来源：http://zhp.fzhhl.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zkg.cqqwz.cn

[R37] 把输出赋给变量
来源：http://gbv.svipenyu.cn

files=$(ls -1)
来源：http://yoo.smart0.xyz

[R38] 管道串联
来源：http://plg.c1oappe.top

cat a.txt | grep -i error | wc -l
来源：http://gxp.guowangkeji.top

[R39] 重定向标准输出与错误
来源：http://eru.zycfv.cn

cmd > out.log 2>&1
来源：http://lut.tianlin.xyz

[R40] 追加写日志
来源：http://lgg.zdbjq.cn

echo "log" >> out.log
来源：http://ezw.quarkkingdee.top

[R41] 丢弃输出
来源：http://mdw.gotoacloud.top

cmd >/dev/null 2>&1
来源：http://qgd.jlsjyb.cn

[R42] 输入重定向
来源：http://yxb.yonumen.top

wc -l < a.txt
来源：http://luu.xinyue.icu

[R43] 按名字查找文件
来源：http://xut.xylfe.cn

find . -name "*.log" -type f
来源：http://tjj.hesvh.cn

[R44] 按修改时间查找
来源：http://emq.ydzc1.top

find . -mtime -7 -type f
来源：http://gns.quarkkingdee.top

[R45] 批量删除
来源：http://evr.hesvh.cn

find . -name "*.tmp" -delete
来源：http://mcd.andypj.xyz

[R46] 递归替换文件内容
来源：http://efg.xinyue.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gzi.xuanzx.com

[R47] sed 单行替换
来源：http://eno.iojbl.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mon.fktsv.cn

[R48] awk 取指定列
来源：http://qff.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://hgh.vehdjk.com

[R49] awk 带条件
来源：http://vjs.havefunace.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zcb.zhiwuduotai.top

[R50] awk 求和
来源：http://ppc.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bmc.aizwys.cn

[R51] 排序去重取前几
来源：http://duw.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tzd.bjfxy.top

[R52] 统计行数
来源：http://mzy.xylfe.cn

wc -l a.txt
来源：http://pib.jinghuilouyu.cn

[R53] 查看文件头与实时尾
来源：http://mzu.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gel.sweek.top

[R54] 比较两个文件
来源：http://obs.ybcxt.top

diff a.txt b.txt
来源：http://xtz.zhongyouzk.top

[R55] 压缩与解压
来源：http://qzs.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cfu.yj202588.top

[R56] 远程拷贝
来源：http://fdd.zhengqikj.top

scp file user@host:/path/
来源：http://wcx.316326.xyz

[R57] 远程执行命令
来源：http://otx.hongshengwenyu.top

ssh user@host 'uptime'
来源：http://zub.quarkkingdee.top

[R58] 下载文件
来源：http://ome.vqdsnc.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kps.ctjpmb.com

[R59] 发 POST JSON
来源：http://wwp.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dxh.fzhhl.top

[R60] 只看 HTTP 状态码
来源：http://giu.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yyh.yj20258.top

[R61] 磁盘占用
来源：http://hgx.xylfe.cn

df -h;  du -sh *
来源：http://nph.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://fml.fengsongda.top

du -ah . | sort -rh | head -10
来源：http://mdo.zycfv.cn

[R63] 内存与进程
来源：http://htd.yonumen.top

free -h;  ps aux | grep nginx
来源：http://oxg.ppjwa.cn

[R64] 结束进程
来源：http://wag.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://fpx.yj202588.top

[R65] 查看端口占用
来源：http://kxm.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hdx.nanxinkj.top

[R66] 定时任务
来源：http://mgc.smart0.xyz

crontab -e;  crontab -l
来源：http://oga.shanyushiyangkeji.top

[R67] 生成随机十六进制串
来源：http://esp.yueranfly.top

openssl rand -hex 16
来源：http://cil.tianlin.xyz

[R68] 计算文件校验值
来源：http://tja.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://qcq.yvedp.cn

[R69] 生成随机密码
来源：http://mhf.cdnleiting.top

head -c 16 /dev/urandom | base64
来源：http://saj.iojbl.cn

[R70] 时间戳与互转
来源：http://vpu.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://iom.jinghuilouyu.cn

[R71] 日期格式化
来源：http://oqw.smart0.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://key.gogol.net.cn

[R72] 等待端口就绪
来源：http://hut.xingfuxueyuan.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://ark.mhx1999.top

[R73] 分割大日志
来源：http://uvf.jinqigfzy.top

split -l 1000 big.log part_
来源：http://ted.daria6918.cn

[R74] 批量重命名
来源：http://lkp.ivvv.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ffc.fktsv.cn

[R75] 导出环境变量
来源：http://jsw.shanyushiyangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://uuc.vehdjk.com

[R76] 使用临时文件
来源：http://jxp.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ubh.vehdjk.com

[R77] 读取用户输入
来源：http://zfa.zhiwuduotai.top

read -rp "请输入: " ans
来源：http://knd.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://lcd.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tgz.smart0.xyz

[R79] 解析命令行选项
来源：http://gaj.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ssc.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://per.xingfuxueyuan.xyz

time ./run.sh
来源：http://fma.zhongyouzk.top

================================================================================
来源：http://bja.shanyushiyangtech.top

S. C / C++ 专题
来源：http://evo.shzxlz.cn

================================================================================
来源：http://sli.iojbl.cn

[S01] C：Hello World
来源：http://ecs.uphjek.com

#include <stdio.h>
来源：http://wct.ppjwa.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://idb.yuxming.cn

[S02] C：变量与格式化输出
来源：http://apw.xziqi.cn

int a = 10; printf("%d\n", a);
来源：http://qla.vehdjk.com

[S03] C：读入整数
来源：http://ocg.gzhubu.top

int x; scanf("%d", &x);
来源：http://yzh.ywan-chungtsiang.top

[S04] C：字符串复制
来源：http://vzt.nwbrower.top

char dst[32]; strcpy(dst, "hi");
来源：http://tdp.vqdsnc.cn

[S05] C：字符串长度
来源：http://fke.sjlbkw.cn

strlen(s)
来源：http://phe.hysaishi.cn

[S06] C：字符串比较
来源：http://ygs.iojbl.cn

strcmp(a, b) == 0
来源：http://ykf.zdbjq.cn

[S07] C：数组遍历求和
来源：http://fbt.havefunace.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://btz.aizwys.cn

[S08] C：动态内存分配与释放
来源：http://nux.c1oappe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://buo.uphjek.com

[S09] C：结构体定义与初始化
来源：http://uvu.tian-w.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://seh.guannengcc.top

[S10] C：指针与解引用
来源：http://aeg.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://scf.chenlongwang.top

[S11] C：逐行读文件
来源：http://avz.zhixingplan.top

FILE *f = fopen("a.txt", "r");
来源：http://bsg.zhongyouzk.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dnv.316326.xyz

fclose(f);
来源：http://cxj.zhixingplan.top

[S12] C：写文件
来源：http://wee.chenlongwang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ebf.epnwcf.com

[S13] C：宏定义
来源：http://cyw.ywan-chungtsiang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zxp.jiagoushi.top

[S14] C：枚举
来源：http://fca.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://rbf.dianchejie.cn

[S15] C：类型转换
来源：http://nni.nwbrower.top

(double) a / b
来源：http://xcp.wangdashe.top

[S16] C：位操作置位
来源：http://fjv.yj202588.top

x |= (1 << 3);
来源：http://cjp.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://tck.0kj1m.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kag.xuetiantiany.cn

[S18] C：命令行参数
来源：http://jvk.tianlin.xyz

int main(int argc, char **argv)
来源：http://uqc.9152youxi.cn

[S19] C：快速排序
来源：http://rji.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ouu.hammf.cn

[S20] C：二分查找
来源：http://txt.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bkf.yj20258.top

[S21] C：字符类别判断
来源：http://cra.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dzw.52xcode.cn

[S22] C：字符串转数字
来源：http://fhf.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://mby.9152youxi.cn

[S23] C：随机数
来源：http://nbf.andypj.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://jbc.ivvv.top

[S24] C：获取本地时间
来源：http://gse.fzhhl.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eiv.aibaodan.cn

[S25] C：内存拷贝
来源：http://pih.zhoulong.xyz

memcpy(dst, src, n);
来源：http://cyz.hfpthk.cn

[S26] C：内存清零
来源：http://dnr.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://aob.zhoulong.xyz

[S27] C：定义常量
来源：http://xhg.kuanghao11.cn

const double PI = 3.14159;
来源：http://ivm.guannengcc.top

[S28] C：静态变量
来源：http://vky.jianghu66.top

static int counter = 0;
来源：http://fqi.jyoumei.cn

[S29] C：变参函数
来源：http://tgp.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://msn.cucudq.cn

[S30] C：头文件保护
来源：http://hth.andypj.xyz


<!-- 参考信息 -->