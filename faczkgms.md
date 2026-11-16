代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rtc.cashguo.top

[Q58] 累计求和
来源：http://mzo.daria6918.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xqo.jyoumei.cn

[Q59] 分组内累计
来源：http://xbx.hysaishi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fce.xuetiantiany.cn

[Q60] 取上一行 / 下一行
来源：http://wrz.quarkkingdee.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bap.jyoumei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bkv.jianghu66.top

[Q61] 移动平均
来源：http://hei.birdmap.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ezz.tianlin.xyz

[Q62] 分组占比
来源：http://qns.xinyue.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://btu.guowangkeji.top

[Q63] 开启事务
来源：http://ilh.gaohongyu789.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sry.tian-w.cn

[Q64] 提交事务
来源：http://khh.ehwqpu.com

COMMIT;
来源：http://moz.zdqjudy.top

[Q65] 回滚事务
来源：http://fac.gotoacloud.top

ROLLBACK;
来源：http://ikj.vehdjk.com

[Q66] 行锁查询
来源：http://nws.redwolf501.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pue.zhongyouzk.top

[Q67] 设置隔离级别
来源：http://btc.xziqi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nxr.jyoumei.cn

[Q68] 保存点
来源：http://bac.jiagoushi.top

SAVEPOINT sp1;
来源：http://zgb.ivvv.top

ROLLBACK TO sp1;
来源：http://kty.cheryme.top

[Q69] 查看执行计划
来源：http://ype.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uoh.tianlin.xyz

[Q70] 更新统计信息
来源：http://dmg.hcnkem.com

ANALYZE TABLE users;
来源：http://afc.hammf.cn

[Q71] 查看建表语句
来源：http://atf.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pvs.sxryk.cn

[Q72] 查看索引
来源：http://xnf.birdmap.top

SHOW INDEX FROM users;
来源：http://rbv.gogol.net.cn

[Q73] 查看表状态
来源：http://fqz.ehwqpu.com

SHOW TABLE STATUS LIKE 'users';
来源：http://qha.yueranfly.top

[Q74] 强制使用索引
来源：http://dwi.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ltz.ppjwa.cn

[Q75] 日期格式化
来源：http://juj.52xcode.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lao.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cut.yvedp.cn

[Q76] 按天统计
来源：http://djk.vqdsnc.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mkm.iojbl.cn

[Q77] 时间加减
来源：http://fxw.hnqzz.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ugq.ydzc1.top

[Q78] 当前时间
来源：http://geb.shzxlz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qra.gaohongyu789.top

[Q79] 字符串拼接
来源：http://fqj.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cut.jqgufenzy.top

[Q80] 字符串截取
来源：http://jlm.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fho.cqqwz.cn

[Q81] 字符串替换
来源：http://ssn.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wqp.jinqigufen.top

[Q82] 字符长度与字节长度
来源：http://hhb.hongshengwenyu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wpj.guannengcc.top

[Q83] 大小写转换
来源：http://jcj.xuetiantiany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gmk.gotoacloud.top

[Q84] 去除首尾空格
来源：http://vsh.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://ypg.jinqigufen.top

[Q85] 数值取整
来源：http://xjr.fengsongda.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nec.zhijiandao.cn

[Q86] 读取 JSON 字段
来源：http://gez.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cxi.jyoumei.cn

[Q87] JSON 字段做条件
来源：http://fxm.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://amu.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://okc.guowangkeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dkv.hongshengwenyu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gsd.zdbjq.cn

[Q89] 判断表是否存在
来源：http://mxw.chenjidiqi.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mmc.haohaochexian.top

[Q90] 生成序号列
来源：http://ljf.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://txh.zhongyouzk.top

================================================================================
来源：http://jii.cucudq.cn

R. Bash 专题
来源：http://rdf.gaohongyu789.top

================================================================================
来源：http://pjb.wangdashe.top

[R01] shebang 与严格模式
来源：http://mba.xinyue.icu

#!/usr/bin/env bash
来源：http://rsd.sweek.top

set -euo pipefail
来源：http://tmp.316326.xyz

[R02] 变量赋值与使用
来源：http://ect.sxryk.cn

name="Tom"; echo "$name"
来源：http://waj.jianghu66.top

[R03] 只读变量
来源：http://lzd.redwolf501.top

readonly PI=3.14
来源：http://rld.birdmap.top

[R04] 位置参数
来源：http://vmn.zhijiandao.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hqx.zhaomingkeji.xyz

[R05] 参数默认值
来源：http://efo.hnxiangtu.top

name="${1:-default}"
来源：http://txd.svipenyu.cn

[R06] 判断命令是否存在
来源：http://jvp.gogol.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dgn.sxryk.cn

[R07] if 判断文件
来源：http://itf.aizwys.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uwe.redwolf501.top

[R08] 数值比较
来源：http://dch.vehdjk.com

if (( a > b )); then echo "a 更大"; fi
来源：http://oqd.nanxuanxn.top

[R09] 字符串比较
来源：http://acy.jinghuilouyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vhd.xziqi.cn

[R10] 正则匹配
来源：http://dyp.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dyc.yonumen.top

[R11] case 多分支
来源：http://nti.vehdjk.com

case "$1" in
来源：http://oot.iojbl.cn

start) echo "启动" ;;
来源：http://tar.daxiang520.top

stop)  echo "停止" ;;
来源：http://uag.fehbvm.com

*)     echo "未知命令" ;;
来源：http://bha.jinyuanbaomall.cn

esac
来源：http://wbk.shanyushiyangkeji.top

[R12] for 遍历文件
来源：http://pzo.gotoacloud.top

for f in *.txt; do echo "$f"; done
来源：http://cww.shanyushiyangtech.top

[R13] for 计数循环
来源：http://yhk.hfpthk.cn

for i in {1..10}; do echo "$i"; done
来源：http://clo.birdmap.top

[R14] C 风格 for
来源：http://cal.jianghu66.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gla.hysaishi.cn

[R15] while 逐行读文件
来源：http://wgi.shanyushiyangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://llu.ybcxt.top

[R16] until 等待条件
来源：http://iax.meibo888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hpj.hcnkem.com

[R17] 数组定义与取值
来源：http://eds.tianlin.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://rwu.feifeiyinyue.top

[R18] 遍历数组
来源：http://kid.hywenlv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eye.sjlbkw.cn

[R19] 数组长度
来源：http://obf.cdnleiting.top

echo "${#arr[@]}"
来源：http://fak.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://alz.zycfv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://foc.hammf.cn

[R21] 字符串长度
来源：http://fnf.kuanghao11.cn

echo "${#s}"
来源：http://zbl.pengpengdd.cyou

[R22] 截取子串
来源：http://qqv.52xcode.cn

echo "${s:0:5}"
来源：http://usr.tianlin.xyz

[R23] 字符串替换
来源：http://lzc.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lnp.yj20258888.top

[R24] 大小写转换
来源：http://exz.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mpw.shanyushiyangtech.top

[R25] 去后缀 / 去前缀
来源：http://maq.gzhubu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tuj.ydzc1.top

[R26] 命令替换
来源：http://teg.yonumen.top

now=$(date +%F); echo "$now"
来源：http://jsj.xuetiantiany.cn

[R27] 算术展开
来源：http://cau.pycfn.com

echo $((1 + 2 * 3))
来源：http://hpc.jinghuilouyu.cn

[R28] 浮点运算
来源：http://hta.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://mfr.yj20258888.top

[R29] 定义函数
来源：http://avb.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dbn.svipenyu.cn

[R30] 函数返回状态码
来源：http://yev.fengsongda.top

f() { return 0; }; f || echo "失败了"
来源：http://bwh.cheryme.top

[R31] 局部变量
来源：http://xsf.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://hcd.cucudq.cn

[R32] 参数个数校验
来源：http://vjl.ppjwa.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jcc.dashuyun.cn

[R33] 捕获错误并提示行号
来源：http://kzb.quarkkingdee.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aqm.jinyuanbaomall.cn

[R34] 退出时清理
来源：http://mio.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://nak.xuanzx.com

[R35] 后台执行并等待
来源：http://spz.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hxy.hcnkem.com

[R36] 并发执行多个任务
来源：http://jug.daxiang520.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bch.yj202588.top

[R37] 把输出赋给变量
来源：http://xvz.aizwys.cn

files=$(ls -1)
来源：http://sds.havefunace.top

[R38] 管道串联
来源：http://dru.svipenyu.cn

cat a.txt | grep -i error | wc -l
来源：http://xus.cheryme.top

[R39] 重定向标准输出与错误
来源：http://wwk.9152youxi.cn

cmd > out.log 2>&1
来源：http://kaf.fengsongda.top

[R40] 追加写日志
来源：http://qck.tarul.cn

echo "log" >> out.log
来源：http://ype.redwolf501.top

[R41] 丢弃输出
来源：http://fdp.zhaomingkeji.xyz

cmd >/dev/null 2>&1
来源：http://xbc.hammf.cn

[R42] 输入重定向
来源：http://pwo.yvedp.cn

wc -l < a.txt
来源：http://whp.zdbjq.cn

[R43] 按名字查找文件
来源：http://clp.jinqigfzy.top

find . -name "*.log" -type f
来源：http://oim.xylfe.cn

[R44] 按修改时间查找
来源：http://kmi.sxryk.cn

find . -mtime -7 -type f
来源：http://vme.guowangkeji.top

[R45] 批量删除
来源：http://ypx.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://aqg.nanxinkj.top

[R46] 递归替换文件内容
来源：http://mlo.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iob.fktsv.cn

[R47] sed 单行替换
来源：http://dfz.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://cpr.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://tth.tanke756.top

awk '{print $1, $3}' a.txt
来源：http://tll.zhijiandao.cn

[R49] awk 带条件
来源：http://mpr.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://btx.yueranfly.top

[R50] awk 求和
来源：http://aay.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://peh.uphjek.com

[R51] 排序去重取前几
来源：http://vet.gogol.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://owe.fanxiaobao.xyz

[R52] 统计行数
来源：http://oor.chenzaomai.com

wc -l a.txt
来源：http://alt.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://iqs.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iad.hnqzz.top

[R54] 比较两个文件
来源：http://ffs.ppjwa.cn

diff a.txt b.txt
来源：http://xta.daxiang520.top

[R55] 压缩与解压
来源：http://muc.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rsb.yongpay.top

[R56] 远程拷贝
来源：http://hjl.jlsjyb.cn

scp file user@host:/path/
来源：http://vie.hywenlv.cn

[R57] 远程执行命令
来源：http://efs.zycfv.cn

ssh user@host 'uptime'
来源：http://tzb.cashguo.top

[R58] 下载文件
来源：http://taq.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qyt.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://fky.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zzk.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://zdr.chenlongwang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hcd.shanyushiyangkeji.top

[R61] 磁盘占用
来源：http://xxw.vqdsnc.cn

df -h;  du -sh *
来源：http://vch.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://vip.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://inq.dianchejie.cn

[R63] 内存与进程
来源：http://gfb.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://afe.zycfv.cn

[R64] 结束进程
来源：http://euc.yanxiufei.cn

kill -9 $(pgrep -f app.py)
来源：http://jxx.ehwqpu.com

[R65] 查看端口占用
来源：http://dhx.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://neg.jqgfzy.top

[R66] 定时任务
来源：http://egd.hammf.cn

crontab -e;  crontab -l
来源：http://gjx.yangfankeji.com

[R67] 生成随机十六进制串
来源：http://rtj.zhixingplan.top

openssl rand -hex 16
来源：http://dxp.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://wpf.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://hvz.tian-w.cn

[R69] 生成随机密码
来源：http://etf.xuetiantiany.cn

head -c 16 /dev/urandom | base64
来源：http://lld.jinqigfzy.top

[R70] 时间戳与互转
来源：http://agj.zhoulong.xyz

date +%s;  date -d @1700000000
来源：http://qek.yongpay.top

[R71] 日期格式化
来源：http://zgo.nanxinkj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://otm.nanxuanxn.top

[R72] 等待端口就绪
来源：http://itb.yvedp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://snf.sufxvd.cn

[R73] 分割大日志
来源：http://oex.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://tsu.shzxlz.cn

[R74] 批量重命名
来源：http://ahn.gaohongyu789.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kax.fanxiaobao.xyz

[R75] 导出环境变量
来源：http://fet.zhiwuduotai.top

export PATH="$HOME/bin:$PATH"
来源：http://qra.jqgufenzy.top

[R76] 使用临时文件
来源：http://pqt.smart0.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fjp.ivvv.top

[R77] 读取用户输入
来源：http://she.sweek.top

read -rp "请输入: " ans
来源：http://egq.chenjidiqi.icu

[R78] 交互式菜单
来源：http://fuy.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mnf.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://hkn.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://frl.fktsv.cn

[R80] 查看脚本执行耗时
来源：http://hzv.ivvv.top

time ./run.sh
来源：http://oor.redwolf501.top

================================================================================
来源：http://flj.jianghu66.top

S. C / C++ 专题
来源：http://qqr.yangfankeji.com

================================================================================
来源：http://pbo.bjfxy.top

[S01] C：Hello World
来源：http://zfk.ivvv.top

#include <stdio.h>
来源：http://ryb.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hoo.yj20258.top

[S02] C：变量与格式化输出
来源：http://ejb.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://obp.bjfxy.top

[S03] C：读入整数
来源：http://yxf.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://rrm.yonumen.top

[S04] C：字符串复制
来源：http://xij.birdmap.top

char dst[32]; strcpy(dst, "hi");
来源：http://jrb.zhiwuduotai.top

[S05] C：字符串长度
来源：http://ors.jinghuilouyu.cn

strlen(s)
来源：http://ftb.hcnkem.com

[S06] C：字符串比较
来源：http://kkv.bbcook.cn

strcmp(a, b) == 0
来源：http://xpq.jlsjyb.cn

[S07] C：数组遍历求和
来源：http://mxp.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://log.zhixingplan.top

[S08] C：动态内存分配与释放
来源：http://ubd.ivvv.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wxw.guowangkeji.top

[S09] C：结构体定义与初始化
来源：http://ipp.jiagoushi.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qaq.ctjpmb.com

[S10] C：指针与解引用
来源：http://wiu.wangshuangyany.cn

int *p = &a;  *p = 5;
来源：http://tqd.tian-w.cn

[S11] C：逐行读文件
来源：http://vxw.quarkkingdee.top

FILE *f = fopen("a.txt", "r");
来源：http://tch.cashguo.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vrs.ybcxt.top

fclose(f);
来源：http://bfi.hywenlv.cn

[S12] C：写文件
来源：http://nxq.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wrr.9152youxi.cn

[S13] C：宏定义
来源：http://cyu.sxryk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ifh.zhongyouzk.top

[S14] C：枚举
来源：http://bcx.yfazqb.com

enum Color { RED, GREEN, BLUE };
来源：http://iiw.tarul.cn

[S15] C：类型转换
来源：http://qwr.pengpengdd.cyou

(double) a / b
来源：http://fqs.epnwcf.com

[S16] C：位操作置位
来源：http://wkt.chenjidiqi.icu

x |= (1 << 3);
来源：http://tkm.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://bmp.jiagoushi.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zrh.ctjpmb.com

[S18] C：命令行参数
来源：http://jzt.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://tik.yj20258888.top

[S19] C：快速排序
来源：http://nfw.hesvh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gnu.quarkkingdee.top

[S20] C：二分查找
来源：http://fre.nanxuanxn.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tfl.jyoumei.cn

[S21] C：字符类别判断
来源：http://akd.jlsjyb.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hfo.ppjwa.cn

[S22] C：字符串转数字
来源：http://evn.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qqo.xziqi.cn

[S23] C：随机数
来源：http://fbj.ehwqpu.com

srand(time(NULL));  int r = rand() % 100;
来源：http://kuj.jinghuilouyu.cn

[S24] C：获取本地时间
来源：http://xxy.bbcook.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eis.hnqzz.top

[S25] C：内存拷贝
来源：http://ych.gotoacloud.top

memcpy(dst, src, n);
来源：http://zxu.ppjwa.cn

[S26] C：内存清零
来源：http://fco.quarkkingdee.top

memset(a, 0, sizeof a);
来源：http://eot.hysaishi.cn

[S27] C：定义常量
来源：http://zpj.316326.xyz

const double PI = 3.14159;
来源：http://iuo.ppjwa.cn

[S28] C：静态变量
来源：http://anz.uphjek.com


<!-- 参考信息 -->