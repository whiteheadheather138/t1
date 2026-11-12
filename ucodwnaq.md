代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ngq.cdnleiting.top

[Q58] 累计求和
来源：http://jje.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qot.yfazqb.com

[Q59] 分组内累计
来源：http://xow.bjfxy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bpo.guowangkeji.top

[Q60] 取上一行 / 下一行
来源：http://dso.nwbrower.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ffk.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fmz.yueranfly.top

[Q61] 移动平均
来源：http://hup.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yqb.daxiang520.top

[Q62] 分组占比
来源：http://bub.gaohongyu789.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rzh.xziqi.cn

[Q63] 开启事务
来源：http://sri.hcnkem.com

START TRANSACTION;                -- 或 BEGIN
来源：http://yku.tarul.cn

[Q64] 提交事务
来源：http://tnp.ydzc1.top

COMMIT;
来源：http://ien.ctjpmb.com

[Q65] 回滚事务
来源：http://urt.xziqi.cn

ROLLBACK;
来源：http://kaf.smart0.xyz

[Q66] 行锁查询
来源：http://qbz.jqgfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xxa.mhx1999.top

[Q67] 设置隔离级别
来源：http://eyj.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gob.gaohongyu789.top

[Q68] 保存点
来源：http://vlk.sxryk.cn

SAVEPOINT sp1;
来源：http://ngw.ctjpmb.com

ROLLBACK TO sp1;
来源：http://jfy.ppjwa.cn

[Q69] 查看执行计划
来源：http://tjj.fanxiaobao.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tjf.guowangkeji.top

[Q70] 更新统计信息
来源：http://fgy.daria6918.cn

ANALYZE TABLE users;
来源：http://pgj.yueranfly.top

[Q71] 查看建表语句
来源：http://axp.gotoacloud.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dyj.epnwcf.com

[Q72] 查看索引
来源：http://dgd.tarul.cn

SHOW INDEX FROM users;
来源：http://qwu.meibo888.top

[Q73] 查看表状态
来源：http://guf.yj20258888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ocb.sjlbkw.cn

[Q74] 强制使用索引
来源：http://sse.yueranfly.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nvl.c1oappe.top

[Q75] 日期格式化
来源：http://mki.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zbj.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://szb.jinghuilouyu.cn

[Q76] 按天统计
来源：http://ikd.tarul.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ksh.xziqi.cn

[Q77] 时间加减
来源：http://aqx.andypj.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bbq.sufxvd.cn

[Q78] 当前时间
来源：http://atf.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://isk.yanxiufei.cn

[Q79] 字符串拼接
来源：http://jgr.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ssc.gaohongyu789.top

[Q80] 字符串截取
来源：http://art.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://trd.zhijiandao.cn

[Q81] 字符串替换
来源：http://dhn.hammf.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hcj.xuanzx.com

[Q82] 字符长度与字节长度
来源：http://abk.yongpay.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iim.zhongyouzk.top

[Q83] 大小写转换
来源：http://wds.shanyushiyangtech.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lvw.tian-w.cn

[Q84] 去除首尾空格
来源：http://jed.zdbjq.cn

SELECT TRIM(name) FROM users;
来源：http://wbl.yanxiufei.cn

[Q85] 数值取整
来源：http://net.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lqs.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://hrd.fengsongda.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fnt.cheryme.top

[Q87] JSON 字段做条件
来源：http://gyx.c1oappe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wfs.zhixingplan.top

[Q88] 行转列（条件聚合）
来源：http://tih.chenzaomai.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vst.pycfn.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yfe.tian-w.cn

[Q89] 判断表是否存在
来源：http://uaa.jlsjyb.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://esn.gzhubu.top

[Q90] 生成序号列
来源：http://upm.jiagoushi.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tvb.yangfankeji.com

================================================================================
来源：http://zde.mhx1999.top

R. Bash 专题
来源：http://spf.quarkkingdee.top

================================================================================
来源：http://lpy.havefunace.top

[R01] shebang 与严格模式
来源：http://ppx.svipenyu.cn

#!/usr/bin/env bash
来源：http://atk.zdbjq.cn

set -euo pipefail
来源：http://pjl.smart0.xyz

[R02] 变量赋值与使用
来源：http://hmh.zhiwuduotai.top

name="Tom"; echo "$name"
来源：http://mdc.nanxinkj.top

[R03] 只读变量
来源：http://uel.ydzc1.top

readonly PI=3.14
来源：http://cyh.quarkkingdee.top

[R04] 位置参数
来源：http://kfq.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mcm.jiagoushi.top

[R05] 参数默认值
来源：http://oqf.yj20258888.top

name="${1:-default}"
来源：http://wdu.jianghu66.top

[R06] 判断命令是否存在
来源：http://zqj.xuetiantiany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wit.316326.xyz

[R07] if 判断文件
来源：http://zms.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pnm.hywenlv.cn

[R08] 数值比较
来源：http://ooj.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ujt.zycfv.cn

[R09] 字符串比较
来源：http://hds.zhijiandao.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pwx.zdbjq.cn

[R10] 正则匹配
来源：http://yyk.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mhx.gotoacloud.top

[R11] case 多分支
来源：http://qko.zycfv.cn

case "$1" in
来源：http://tdy.xziqi.cn

start) echo "启动" ;;
来源：http://xio.meibo888.top

stop)  echo "停止" ;;
来源：http://ece.redwolf501.top

*)     echo "未知命令" ;;
来源：http://awi.zhongyouzk.top

esac
来源：http://mol.jinghuilouyu.cn

[R12] for 遍历文件
来源：http://ikd.ctjpmb.com

for f in *.txt; do echo "$f"; done
来源：http://ulk.vqdsnc.cn

[R13] for 计数循环
来源：http://dtd.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://hvd.gaohongyu789.top

[R14] C 风格 for
来源：http://nri.birdmap.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tqc.zhoulong.xyz

[R15] while 逐行读文件
来源：http://uin.pengpengdd.cyou

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vlw.xuanzx.com

[R16] until 等待条件
来源：http://ohp.316326.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ylk.zdqjudy.top

[R17] 数组定义与取值
来源：http://pod.jinyuanbaomall.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dht.zdbjq.cn

[R18] 遍历数组
来源：http://bza.9152youxi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vid.xuetiantiany.cn

[R19] 数组长度
来源：http://rho.hysaishi.cn

echo "${#arr[@]}"
来源：http://pij.quarkkingdee.top

[R20] 关联数组（字典）
来源：http://mhf.fehbvm.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dsl.fanxiaobao.xyz

[R21] 字符串长度
来源：http://siw.fzhhl.top

echo "${#s}"
来源：http://nfn.zhongyouzk.top

[R22] 截取子串
来源：http://xnn.zdbjq.cn

echo "${s:0:5}"
来源：http://owu.redwolf501.top

[R23] 字符串替换
来源：http://smz.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eet.havefunace.top

[R24] 大小写转换
来源：http://zce.redwolf501.top

echo "${s^^}"; echo "${s,,}"
来源：http://wrc.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://zwo.52xcode.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://onr.xuanzx.com

[R26] 命令替换
来源：http://pgs.hongshengwenyu.top

now=$(date +%F); echo "$now"
来源：http://zba.nanxinkj.top

[R27] 算术展开
来源：http://exz.hnqzz.top

echo $((1 + 2 * 3))
来源：http://mru.zdbjq.cn

[R28] 浮点运算
来源：http://ano.yfazqb.com

echo "scale=2; 10/3" | bc
来源：http://drp.ehwqpu.com

[R29] 定义函数
来源：http://uqn.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hty.nanxinkj.top

[R30] 函数返回状态码
来源：http://cgc.fehbvm.com

f() { return 0; }; f || echo "失败了"
来源：http://zqh.hongshengwenyu.top

[R31] 局部变量
来源：http://wcm.jqgfzy.top

f() { local x=1; echo "$x"; }
来源：http://otu.yj20258.top

[R32] 参数个数校验
来源：http://tyo.hesvh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jxf.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://vus.hywenlv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qqw.hnxiangtu.top

[R34] 退出时清理
来源：http://ffv.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://hea.zdqjudy.top

[R35] 后台执行并等待
来源：http://cxy.cashguo.top

sleep 5 & pid=$!; wait "$pid"
来源：http://aer.ydzc1.top

[R36] 并发执行多个任务
来源：http://tly.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://brp.jianghu66.top

[R37] 把输出赋给变量
来源：http://prh.nanxinkj.top

files=$(ls -1)
来源：http://wrs.gogol.net.cn

[R38] 管道串联
来源：http://qrz.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://wwf.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://trr.nanxinkj.top

cmd > out.log 2>&1
来源：http://ogp.gaohongyu789.top

[R40] 追加写日志
来源：http://xip.guannengcc.top

echo "log" >> out.log
来源：http://qmc.zhaomingkeji.xyz

[R41] 丢弃输出
来源：http://tbs.zhengqikj.top

cmd >/dev/null 2>&1
来源：http://mfu.sweek.top

[R42] 输入重定向
来源：http://dln.yj20258888.top

wc -l < a.txt
来源：http://jgc.meibo888.top

[R43] 按名字查找文件
来源：http://zsd.zdbjq.cn

find . -name "*.log" -type f
来源：http://msb.fehbvm.com

[R44] 按修改时间查找
来源：http://dck.yonumen.top

find . -mtime -7 -type f
来源：http://irm.mhx1999.top

[R45] 批量删除
来源：http://gir.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://zym.jqgfzy.top

[R46] 递归替换文件内容
来源：http://fkg.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://orm.shzxlz.cn

[R47] sed 单行替换
来源：http://ben.gotoacloud.top

sed -i 's/foo/bar/g' a.txt
来源：http://jnh.chenzaomai.com

[R48] awk 取指定列
来源：http://yyt.ppjwa.cn

awk '{print $1, $3}' a.txt
来源：http://hcv.sweek.top

[R49] awk 带条件
来源：http://ncy.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uet.xingfuxueyuan.xyz

[R50] awk 求和
来源：http://mwy.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://pks.dashuyun.cn

[R51] 排序去重取前几
来源：http://bis.c1oappe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rny.jinyuanbaomall.cn

[R52] 统计行数
来源：http://zho.fanxiaobao.xyz

wc -l a.txt
来源：http://igc.daria6918.cn

[R53] 查看文件头与实时尾
来源：http://asl.feifeiyinyue.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://riz.jlsjyb.cn

[R54] 比较两个文件
来源：http://wli.meibo888.top

diff a.txt b.txt
来源：http://stq.yongpay.top

[R55] 压缩与解压
来源：http://tem.gzhubu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tfq.iojbl.cn

[R56] 远程拷贝
来源：http://smo.chenzaomai.com

scp file user@host:/path/
来源：http://vrp.haohaochexian.top

[R57] 远程执行命令
来源：http://bmt.zhixingplan.top

ssh user@host 'uptime'
来源：http://ebm.nanxuanxn.top

[R58] 下载文件
来源：http://jur.gzhubu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dcn.zhixingplan.top

[R59] 发 POST JSON
来源：http://ilk.daxiang520.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fam.yvedp.cn

[R60] 只看 HTTP 状态码
来源：http://pjl.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pbi.epnwcf.com

[R61] 磁盘占用
来源：http://fkw.nanxinkj.top

df -h;  du -sh *
来源：http://epv.cheryme.top

[R62] 找最占空间的文件
来源：http://iij.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://kao.smart0.xyz

[R63] 内存与进程
来源：http://hkp.cqqwz.cn

free -h;  ps aux | grep nginx
来源：http://lxm.gzhubu.top

[R64] 结束进程
来源：http://mds.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://kzb.jlsjyb.cn

[R65] 查看端口占用
来源：http://mpw.gogol.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uah.feifeiyinyue.top

[R66] 定时任务
来源：http://bux.bjfxy.top

crontab -e;  crontab -l
来源：http://nfd.yj20258888.top

[R67] 生成随机十六进制串
来源：http://nte.jiagoushi.top

openssl rand -hex 16
来源：http://eqc.chenzaomai.com

[R68] 计算文件校验值
来源：http://wvn.xinyue.icu

sha256sum a.txt;  md5sum a.txt
来源：http://vew.zhoulong.xyz

[R69] 生成随机密码
来源：http://ujv.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://itr.ybcxt.top

[R70] 时间戳与互转
来源：http://eif.316326.xyz

date +%s;  date -d @1700000000
来源：http://fdo.gzhubu.top

[R71] 日期格式化
来源：http://hbw.birdmap.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cru.gogol.net.cn

[R72] 等待端口就绪
来源：http://jee.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://igz.cheryme.top

[R73] 分割大日志
来源：http://gig.zhengqikj.top

split -l 1000 big.log part_
来源：http://eix.havefunace.top

[R74] 批量重命名
来源：http://bqk.xingfuxueyuan.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ehe.gogol.net.cn

[R75] 导出环境变量
来源：http://ozc.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://tlv.gaohongyu789.top

[R76] 使用临时文件
来源：http://ifs.hnxiangtu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cex.hammf.cn

[R77] 读取用户输入
来源：http://pix.uphjek.com

read -rp "请输入: " ans
来源：http://ywq.ydzc1.top

[R78] 交互式菜单
来源：http://wkv.zhixingplan.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uwc.fehbvm.com

[R79] 解析命令行选项
来源：http://yyp.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vjy.yj20258.top

[R80] 查看脚本执行耗时
来源：http://noz.chenjidiqi.icu

time ./run.sh
来源：http://aof.xinyue.icu

================================================================================
来源：http://cai.svipenyu.cn

S. C / C++ 专题
来源：http://isb.xingfuxueyuan.xyz

================================================================================
来源：http://myo.pycfn.com

[S01] C：Hello World
来源：http://ncz.iojbl.cn

#include <stdio.h>
来源：http://cwr.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gqe.xingfuxueyuan.xyz

[S02] C：变量与格式化输出
来源：http://iay.cheryme.top

int a = 10; printf("%d\n", a);
来源：http://tbp.gogol.net.cn

[S03] C：读入整数
来源：http://hxu.guannengcc.top

int x; scanf("%d", &x);
来源：http://mye.jinghuilouyu.cn

[S04] C：字符串复制
来源：http://lyc.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://dnv.hysaishi.cn

[S05] C：字符串长度
来源：http://wpl.zhaomingkeji.xyz

strlen(s)
来源：http://rzs.yueranfly.top

[S06] C：字符串比较
来源：http://jny.zhijiandao.cn

strcmp(a, b) == 0
来源：http://oiw.wangdashe.top

[S07] C：数组遍历求和
来源：http://wwr.chenjidiqi.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wgp.jyoumei.cn

[S08] C：动态内存分配与释放
来源：http://ugz.ctjpmb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sbf.nwbrower.top

[S09] C：结构体定义与初始化
来源：http://kjn.uphjek.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lud.yfazqb.com

[S10] C：指针与解引用
来源：http://zwb.cashguo.top

int *p = &a;  *p = 5;
来源：http://hkm.shangyingyoupin.top

[S11] C：逐行读文件
来源：http://qju.zhoulong.xyz

FILE *f = fopen("a.txt", "r");
来源：http://smb.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://cjj.birdmap.top

fclose(f);
来源：http://bki.jinghuilouyu.cn

[S12] C：写文件
来源：http://xkg.dianchejie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://glf.jiagoushi.top

[S13] C：宏定义
来源：http://dsu.wangdashe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://roa.zdqjudy.top

[S14] C：枚举
来源：http://dpw.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://peh.yj20258888.top

[S15] C：类型转换
来源：http://opn.yanxiufei.cn

(double) a / b
来源：http://afo.fehbvm.com

[S16] C：位操作置位
来源：http://xyf.cdnleiting.top

x |= (1 << 3);
来源：http://pig.birdmap.top

[S17] C：安全拼接字符串
来源：http://nmw.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tzs.52xcode.cn

[S18] C：命令行参数
来源：http://hvg.zhengqikj.top

int main(int argc, char **argv)
来源：http://wtv.zycfv.cn

[S19] C：快速排序
来源：http://win.pengpengdd.cyou

qsort(a, n, sizeof(int), cmp);
来源：http://xge.yonumen.top

[S20] C：二分查找
来源：http://pee.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://umv.fehbvm.com

[S21] C：字符类别判断
来源：http://ynu.cqqwz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://irg.ppjwa.cn

[S22] C：字符串转数字
来源：http://ksp.jinqigfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://cpg.ctjpmb.com

[S23] C：随机数
来源：http://zbt.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gaq.daria6918.cn

[S24] C：获取本地时间
来源：http://gct.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aiv.aibaodan.cn

[S25] C：内存拷贝
来源：http://syw.gogol.net.cn

memcpy(dst, src, n);
来源：http://kub.uphjek.com

[S26] C：内存清零
来源：http://fmw.hammf.cn

memset(a, 0, sizeof a);
来源：http://mfi.jiagoushi.top

[S27] C：定义常量
来源：http://ksm.hysaishi.cn

const double PI = 3.14159;
来源：http://bxa.andypj.xyz

[S28] C：静态变量
来源：http://oae.jyoumei.cn


<!-- 参考信息 -->