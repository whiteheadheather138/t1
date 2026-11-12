代发 wailian999

[Q61] 移动平均
来源：http://uec.shanyushiyangtech.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mvk.yongpay.top

[Q62] 分组占比
来源：http://ari.daria6918.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ske.shanyushiyangkeji.top

[Q63] 开启事务
来源：http://ywt.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://cws.yongpay.top

[Q64] 提交事务
来源：http://jka.jinghuilouyu.cn

COMMIT;
来源：http://dhd.zhoulong.xyz

[Q65] 回滚事务
来源：http://wyq.hysaishi.cn

ROLLBACK;
来源：http://lhn.xuetiantiany.cn

[Q66] 行锁查询
来源：http://amb.hcnkem.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://whb.zycfv.cn

[Q67] 设置隔离级别
来源：http://vnx.ybcxt.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://scf.havefunace.top

[Q68] 保存点
来源：http://byi.zhongyouzk.top

SAVEPOINT sp1;
来源：http://mqu.fktsv.cn

ROLLBACK TO sp1;
来源：http://euo.hysaishi.cn

[Q69] 查看执行计划
来源：http://alx.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kas.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://tso.xziqi.cn

ANALYZE TABLE users;
来源：http://rlp.jinyuanbaomall.cn

[Q71] 查看建表语句
来源：http://aee.gaohongyu789.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fza.gogol.net.cn

[Q72] 查看索引
来源：http://hui.ehwqpu.com

SHOW INDEX FROM users;
来源：http://amm.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://wep.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lbd.sysykeji.top

[Q74] 强制使用索引
来源：http://tsz.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cts.ctjpmb.com

[Q75] 日期格式化
来源：http://ncs.nanxinkj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dhd.gzhubu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ace.feifeiyinyue.top

[Q76] 按天统计
来源：http://cxo.nanxuanxn.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oaa.uphjek.com

[Q77] 时间加减
来源：http://bik.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eek.ctjpmb.com

[Q78] 当前时间
来源：http://jpg.zhixingplan.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rom.ydzc1.top

[Q79] 字符串拼接
来源：http://rhp.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://opy.cucudq.cn

[Q80] 字符串截取
来源：http://zej.uphjek.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mkn.dianchejie.cn

[Q81] 字符串替换
来源：http://nya.bjfxy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wyo.yj202588.top

[Q82] 字符长度与字节长度
来源：http://vbb.shzxlz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pmb.iojbl.cn

[Q83] 大小写转换
来源：http://ntu.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xqs.vehdjk.com

[Q84] 去除首尾空格
来源：http://odp.redwolf501.top

SELECT TRIM(name) FROM users;
来源：http://bnj.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://wuv.xuetiantiany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oqd.chenjidiqi.icu

[Q86] 读取 JSON 字段
来源：http://xtn.birdmap.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cff.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://uow.dashuyun.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qqu.zhijiandao.cn

[Q88] 行转列（条件聚合）
来源：http://yvy.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rsf.ybcxt.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xvj.daria6918.cn

[Q89] 判断表是否存在
来源：http://lzh.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ilq.andypj.xyz

[Q90] 生成序号列
来源：http://fnn.yongpay.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yoo.svipenyu.cn

================================================================================
来源：http://lpu.sjlbkw.cn

R. Bash 专题
来源：http://nvv.yangfankeji.com

================================================================================
来源：http://hna.aizwys.cn

[R01] shebang 与严格模式
来源：http://ctj.fehbvm.com

#!/usr/bin/env bash
来源：http://otj.0kj1m.cn

set -euo pipefail
来源：http://fyk.jqgfzy.top

[R02] 变量赋值与使用
来源：http://wjn.aizwys.cn

name="Tom"; echo "$name"
来源：http://dvn.xuanzx.com

[R03] 只读变量
来源：http://joe.tianlin.xyz

readonly PI=3.14
来源：http://obd.yfazqb.com

[R04] 位置参数
来源：http://zkm.yfazqb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lpd.xziqi.cn

[R05] 参数默认值
来源：http://kid.mhx1999.top

name="${1:-default}"
来源：http://wyr.jyoumei.cn

[R06] 判断命令是否存在
来源：http://eol.hnxiangtu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gut.cashguo.top

[R07] if 判断文件
来源：http://tkk.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rhk.fzhhl.top

[R08] 数值比较
来源：http://igc.nwbrower.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hre.nwbrower.top

[R09] 字符串比较
来源：http://jit.cucudq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xcp.52xcode.cn

[R10] 正则匹配
来源：http://ohk.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ist.shzxlz.cn

[R11] case 多分支
来源：http://rew.yuxming.cn

case "$1" in
来源：http://hnp.gzhubu.top

start) echo "启动" ;;
来源：http://she.zycfv.cn

stop)  echo "停止" ;;
来源：http://dkn.yfazqb.com

*)     echo "未知命令" ;;
来源：http://nfr.zycfv.cn

esac
来源：http://dwy.shangyingyoupin.top

[R12] for 遍历文件
来源：http://hcy.aibaodan.cn

for f in *.txt; do echo "$f"; done
来源：http://eps.quarkkingdee.top

[R13] for 计数循环
来源：http://isz.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://yjk.kuanghao11.cn

[R14] C 风格 for
来源：http://ibs.zdqjudy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ioc.xuanzx.com

[R15] while 逐行读文件
来源：http://tlz.ctjpmb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dcx.ppjwa.cn

[R16] until 等待条件
来源：http://jqw.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yrn.gotoacloud.top

[R17] 数组定义与取值
来源：http://vld.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://vaj.yanxiufei.cn

[R18] 遍历数组
来源：http://uux.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://guj.zdqjudy.top

[R19] 数组长度
来源：http://wma.xingfuxueyuan.xyz

echo "${#arr[@]}"
来源：http://szx.tanke756.top

[R20] 关联数组（字典）
来源：http://orf.yj20258888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dtl.ehwqpu.com

[R21] 字符串长度
来源：http://ddj.epnwcf.com

echo "${#s}"
来源：http://jlj.hnxiangtu.top

[R22] 截取子串
来源：http://ard.uphjek.com

echo "${s:0:5}"
来源：http://ouk.gaohongyu789.top

[R23] 字符串替换
来源：http://ats.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cub.jianghu66.top

[R24] 大小写转换
来源：http://vks.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://ixk.zycfv.cn

[R25] 去后缀 / 去前缀
来源：http://bhm.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://udg.jinyuanbaomall.cn

[R26] 命令替换
来源：http://quv.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://idr.hfpthk.cn

[R27] 算术展开
来源：http://oqx.mhx1999.top

echo $((1 + 2 * 3))
来源：http://bqe.shzxlz.cn

[R28] 浮点运算
来源：http://ygh.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://oan.fktsv.cn

[R29] 定义函数
来源：http://fnb.svipenyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vhu.quarkkingdee.top

[R30] 函数返回状态码
来源：http://yss.sxryk.cn

f() { return 0; }; f || echo "失败了"
来源：http://jaj.jyoumei.cn

[R31] 局部变量
来源：http://gkj.hammf.cn

f() { local x=1; echo "$x"; }
来源：http://kca.hammf.cn

[R32] 参数个数校验
来源：http://umd.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zso.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://mci.uphjek.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://roo.jinghuilouyu.cn

[R34] 退出时清理
来源：http://vfr.daria6918.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rqi.zhijiandao.cn

[R35] 后台执行并等待
来源：http://aww.tarul.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://idj.jqgufenzy.top

[R36] 并发执行多个任务
来源：http://zyd.tianlin.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://izr.pycfn.com

[R37] 把输出赋给变量
来源：http://jil.yanxiufei.cn

files=$(ls -1)
来源：http://axg.dianchejie.cn

[R38] 管道串联
来源：http://wmt.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://rgf.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://bpq.ivvv.top

cmd > out.log 2>&1
来源：http://nif.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://bgz.hnqzz.top

echo "log" >> out.log
来源：http://ihv.chenlongwang.top

[R41] 丢弃输出
来源：http://nak.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://osz.shuidangran.top

[R42] 输入重定向
来源：http://rze.sufxvd.cn

wc -l < a.txt
来源：http://yyw.yuxming.cn

[R43] 按名字查找文件
来源：http://eib.sjlbkw.cn

find . -name "*.log" -type f
来源：http://qxv.haohaochexian.top

[R44] 按修改时间查找
来源：http://ufy.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://syx.0kj1m.cn

[R45] 批量删除
来源：http://fzd.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://suh.ydzc1.top

[R46] 递归替换文件内容
来源：http://qbb.chenzaomai.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cbd.cashguo.top

[R47] sed 单行替换
来源：http://ovi.zhiwuduotai.top

sed -i 's/foo/bar/g' a.txt
来源：http://rad.jlsjyb.cn

[R48] awk 取指定列
来源：http://tls.birdmap.top

awk '{print $1, $3}' a.txt
来源：http://efz.hongshengwenyu.top

[R49] awk 带条件
来源：http://hnt.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jar.dashuyun.cn

[R50] awk 求和
来源：http://txq.hnqzz.top

awk '{s += $2} END {print s}' a.txt
来源：http://vmz.yangfankeji.com

[R51] 排序去重取前几
来源：http://eck.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://nwg.jinyuanbaomall.cn

[R52] 统计行数
来源：http://qbg.shanyushiyangkeji.top

wc -l a.txt
来源：http://vgd.xuetiantiany.cn

[R53] 查看文件头与实时尾
来源：http://fuk.yangfankeji.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hmn.cheryme.top

[R54] 比较两个文件
来源：http://jbb.shanyushiyangkeji.top

diff a.txt b.txt
来源：http://aeu.jyoumei.cn

[R55] 压缩与解压
来源：http://scn.yuanzhike.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ixa.fanxiaobao.xyz

[R56] 远程拷贝
来源：http://aec.pengpengdd.cyou

scp file user@host:/path/
来源：http://mrk.epnwcf.com

[R57] 远程执行命令
来源：http://mym.zhoulong.xyz

ssh user@host 'uptime'
来源：http://ttz.hywenlv.cn

[R58] 下载文件
来源：http://ick.zhongyouzk.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cuc.fktsv.cn

[R59] 发 POST JSON
来源：http://roc.zhijiandao.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bit.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://jea.iojbl.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oiz.hesvh.cn

[R61] 磁盘占用
来源：http://zdi.nanxinkj.top

df -h;  du -sh *
来源：http://lbu.316326.xyz

[R62] 找最占空间的文件
来源：http://nhg.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://ukd.gogol.net.cn

[R63] 内存与进程
来源：http://gir.vehdjk.com

free -h;  ps aux | grep nginx
来源：http://xkd.jinqigfzy.top

[R64] 结束进程
来源：http://jcc.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://lgc.tarul.cn

[R65] 查看端口占用
来源：http://qen.shanyushiyangtech.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wwa.yangfankeji.com

[R66] 定时任务
来源：http://tms.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://zbg.sufxvd.cn

[R67] 生成随机十六进制串
来源：http://xmu.ctjpmb.com

openssl rand -hex 16
来源：http://bxo.cucudq.cn

[R68] 计算文件校验值
来源：http://wxm.fengsongda.top

sha256sum a.txt;  md5sum a.txt
来源：http://lmo.vehdjk.com

[R69] 生成随机密码
来源：http://qhi.vehdjk.com

head -c 16 /dev/urandom | base64
来源：http://gkc.9152youxi.cn

[R70] 时间戳与互转
来源：http://vqz.sjlbkw.cn

date +%s;  date -d @1700000000
来源：http://xmf.hywenlv.cn

[R71] 日期格式化
来源：http://ltk.birdmap.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sdk.nanxinkj.top

[R72] 等待端口就绪
来源：http://idu.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://klh.nanxinkj.top

[R73] 分割大日志
来源：http://rbn.hywenlv.cn

split -l 1000 big.log part_
来源：http://tkp.shangyingyoupin.top

[R74] 批量重命名
来源：http://arx.jinghuilouyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://esf.hywenlv.cn

[R75] 导出环境变量
来源：http://vld.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://ngf.wangdashe.top

[R76] 使用临时文件
来源：http://akr.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oaw.ehwqpu.com

[R77] 读取用户输入
来源：http://lry.gotoacloud.top

read -rp "请输入: " ans
来源：http://rit.kuanghao11.cn

[R78] 交互式菜单
来源：http://gcg.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hfy.cheryme.top

[R79] 解析命令行选项
来源：http://rwd.hfpthk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dgn.hnqzz.top

[R80] 查看脚本执行耗时
来源：http://ipw.nwbrower.top

time ./run.sh
来源：http://fjb.jqgfzy.top

================================================================================
来源：http://vit.hysaishi.cn

S. C / C++ 专题
来源：http://hep.sjlbkw.cn

================================================================================
来源：http://msg.hammf.cn

[S01] C：Hello World
来源：http://vbt.zhixingplan.top

#include <stdio.h>
来源：http://sgh.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rkd.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://suz.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://qwu.quarkkingdee.top

[S03] C：读入整数
来源：http://gsn.tanke756.top

int x; scanf("%d", &x);
来源：http://vxz.zhengqikj.top

[S04] C：字符串复制
来源：http://yvk.yj20258.top

char dst[32]; strcpy(dst, "hi");
来源：http://qel.mhx1999.top

[S05] C：字符串长度
来源：http://vfi.chenlongwang.top

strlen(s)
来源：http://ctw.yuanzhike.top

[S06] C：字符串比较
来源：http://ple.sufxvd.cn

strcmp(a, b) == 0
来源：http://gqt.shanyushiyangkeji.top

[S07] C：数组遍历求和
来源：http://oum.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wwj.cheryme.top

[S08] C：动态内存分配与释放
来源：http://aqs.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aap.vehdjk.com

[S09] C：结构体定义与初始化
来源：http://fqj.gotoacloud.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://npg.bbcook.cn

[S10] C：指针与解引用
来源：http://hwr.feifeiyinyue.top

int *p = &a;  *p = 5;
来源：http://lme.zhijiandao.cn

[S11] C：逐行读文件
来源：http://fzk.smart0.xyz

FILE *f = fopen("a.txt", "r");
来源：http://gye.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jko.jinghuilouyu.cn

fclose(f);
来源：http://ntt.xingfuxueyuan.xyz

[S12] C：写文件
来源：http://jbp.bbcook.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tic.fktsv.cn

[S13] C：宏定义
来源：http://axw.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yqy.shanyushiyangkeji.top

[S14] C：枚举
来源：http://hoy.redwolf501.top

enum Color { RED, GREEN, BLUE };
来源：http://lmi.nanxinkj.top

[S15] C：类型转换
来源：http://mot.fktsv.cn

(double) a / b
来源：http://zdy.cdnleiting.top

[S16] C：位操作置位
来源：http://mvm.dashuyun.cn

x |= (1 << 3);
来源：http://nsp.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://bih.zhiwuduotai.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://udt.meibo888.top

[S18] C：命令行参数
来源：http://gmc.cdnleiting.top

int main(int argc, char **argv)
来源：http://wpz.jlsjyb.cn

[S19] C：快速排序
来源：http://uql.nanxuanxn.top

qsort(a, n, sizeof(int), cmp);
来源：http://vrk.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://wvw.ivvv.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rgt.sxryk.cn

[S21] C：字符类别判断
来源：http://yoi.bbcook.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://caf.yj20258.top

[S22] C：字符串转数字
来源：http://rcz.jinghuilouyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jpk.fengsongda.top

[S23] C：随机数
来源：http://awx.jqgfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://moe.yj20258.top

[S24] C：获取本地时间
来源：http://nwi.shuidangran.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fix.tarul.cn

[S25] C：内存拷贝
来源：http://vxh.yj20258888.top

memcpy(dst, src, n);
来源：http://vpz.yuxming.cn

[S26] C：内存清零
来源：http://dpq.0kj1m.cn

memset(a, 0, sizeof a);
来源：http://loc.shanyushiyangtech.top

[S27] C：定义常量
来源：http://dny.9152youxi.cn

const double PI = 3.14159;
来源：http://vln.epnwcf.com

[S28] C：静态变量
来源：http://sxv.xingfuxueyuan.xyz

static int counter = 0;
来源：http://boo.9152youxi.cn

[S29] C：变参函数
来源：http://hlp.snrcjt.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ndq.jinqigfzy.top

[S30] C：头文件保护
来源：http://mra.316326.xyz

#ifndef X_H
来源：http://igw.sysykeji.top

#define X_H
来源：http://ogb.daria6918.cn

#endif
来源：http://bmy.zhengqikj.top

[S31] C++：Hello World
来源：http://ups.zycfv.cn


<!-- 参考信息 -->