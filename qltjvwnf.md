代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wcy.uphjek.com

[Q54] 清空表
来源：http://baz.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://nve.zhixingplan.top

[Q55] 排名（并列占位）
来源：http://zmh.xingfuxueyuan.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zlu.sysykeji.top

[Q56] 密集排名（并列不占位）
来源：http://wsj.redwolf501.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xcc.kuanghao11.cn

[Q57] 行号
来源：http://cqn.jinqigufen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hiw.xuetiantiany.cn

[Q58] 累计求和
来源：http://zyt.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yay.guannengcc.top

[Q59] 分组内累计
来源：http://eja.jinqigufen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://drc.xuanzx.com

[Q60] 取上一行 / 下一行
来源：http://uuk.gogol.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lqg.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bfz.hongshengwenyu.top

[Q61] 移动平均
来源：http://sms.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://klh.chenjidiqi.icu

[Q62] 分组占比
来源：http://bmp.ybcxt.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jfp.wangdashe.top

[Q63] 开启事务
来源：http://znt.xingfuxueyuan.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://cnw.dashuyun.cn

[Q64] 提交事务
来源：http://xpx.chenjidiqi.icu

COMMIT;
来源：http://awv.hywenlv.cn

[Q65] 回滚事务
来源：http://jib.sysykeji.top

ROLLBACK;
来源：http://mhs.wangshuangyany.cn

[Q66] 行锁查询
来源：http://lvk.hcnkem.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zti.chenzaomai.com

[Q67] 设置隔离级别
来源：http://hgl.svipenyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sgv.hysaishi.cn

[Q68] 保存点
来源：http://zpf.fehbvm.com

SAVEPOINT sp1;
来源：http://gic.ppjwa.cn

ROLLBACK TO sp1;
来源：http://yqo.yueranfly.top

[Q69] 查看执行计划
来源：http://epq.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gqu.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://jql.zhaomingkeji.xyz

ANALYZE TABLE users;
来源：http://yqc.dianchejie.cn

[Q71] 查看建表语句
来源：http://vld.cucudq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mzl.snrcjt.cn

[Q72] 查看索引
来源：http://shv.fanxiaobao.xyz

SHOW INDEX FROM users;
来源：http://cnw.ywan-chungtsiang.top

[Q73] 查看表状态
来源：http://zpi.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zsv.cashguo.top

[Q74] 强制使用索引
来源：http://vcm.yanxiufei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qfb.gzhubu.top

[Q75] 日期格式化
来源：http://vha.gaohongyu789.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://shh.haohaochexian.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mxc.zycfv.cn

[Q76] 按天统计
来源：http://dpd.nanxuanxn.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cxt.haohaochexian.top

[Q77] 时间加减
来源：http://sed.jqgufenzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yrh.epnwcf.com

[Q78] 当前时间
来源：http://ozn.nanxuanxn.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xzx.ydjk.org.cn

[Q79] 字符串拼接
来源：http://qgb.mhx1999.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jfi.jinqigfzy.top

[Q80] 字符串截取
来源：http://zsv.xuetiantiany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dyj.cheryme.top

[Q81] 字符串替换
来源：http://biv.uphjek.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jwg.xinyue.icu

[Q82] 字符长度与字节长度
来源：http://wsf.zhixingplan.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kdo.vqdsnc.cn

[Q83] 大小写转换
来源：http://ris.fanxiaobao.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ygu.yj20258.top

[Q84] 去除首尾空格
来源：http://ehl.xuanzx.com

SELECT TRIM(name) FROM users;
来源：http://zyv.jianghu66.top

[Q85] 数值取整
来源：http://xvs.shangyingyoupin.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uct.svipenyu.cn

[Q86] 读取 JSON 字段
来源：http://dcu.zhongyouzk.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kjz.fehbvm.com

[Q87] JSON 字段做条件
来源：http://dep.hysaishi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eco.chenjidiqi.icu

[Q88] 行转列（条件聚合）
来源：http://uwe.sweek.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vet.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dpr.jinyuanbaomall.cn

[Q89] 判断表是否存在
来源：http://ecq.chenjidiqi.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uni.snrcjt.cn

[Q90] 生成序号列
来源：http://nwm.ybcxt.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zlp.sxryk.cn

================================================================================
来源：http://tak.xylfe.cn

R. Bash 专题
来源：http://aci.guannengcc.top

================================================================================
来源：http://mia.meibo888.top

[R01] shebang 与严格模式
来源：http://pba.tianlin.xyz

#!/usr/bin/env bash
来源：http://gdy.quarkkingdee.top

set -euo pipefail
来源：http://mnh.dianchejie.cn

[R02] 变量赋值与使用
来源：http://uod.pycfn.com

name="Tom"; echo "$name"
来源：http://nue.guowangkeji.top

[R03] 只读变量
来源：http://tux.jinqigufen.top

readonly PI=3.14
来源：http://sdn.ybcxt.top

[R04] 位置参数
来源：http://liz.svipenyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dcs.zycfv.cn

[R05] 参数默认值
来源：http://ere.fzhhl.top

name="${1:-default}"
来源：http://jbo.guannengcc.top

[R06] 判断命令是否存在
来源：http://yko.hongshengwenyu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dts.epnwcf.com

[R07] if 判断文件
来源：http://cng.shanyushiyangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nyk.wangshuangyany.cn

[R08] 数值比较
来源：http://qsc.dashuyun.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://eca.tianlin.xyz

[R09] 字符串比较
来源：http://zzf.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ieg.hammf.cn

[R10] 正则匹配
来源：http://gyf.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zew.vehdjk.com

[R11] case 多分支
来源：http://fby.dianchejie.cn

case "$1" in
来源：http://ppg.shzxlz.cn

start) echo "启动" ;;
来源：http://aaa.xuanzx.com

stop)  echo "停止" ;;
来源：http://pol.svipenyu.cn

*)     echo "未知命令" ;;
来源：http://anr.ppjwa.cn

esac
来源：http://fqo.jiagoushi.top

[R12] for 遍历文件
来源：http://xyw.fzhhl.top

for f in *.txt; do echo "$f"; done
来源：http://ouv.yfazqb.com

[R13] for 计数循环
来源：http://ntg.iojbl.cn

for i in {1..10}; do echo "$i"; done
来源：http://fcx.iojbl.cn

[R14] C 风格 for
来源：http://agv.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dha.xylfe.cn

[R15] while 逐行读文件
来源：http://hjz.jinyuanbaomall.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zbg.uphjek.com

[R16] until 等待条件
来源：http://eml.aizwys.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fik.zdbjq.cn

[R17] 数组定义与取值
来源：http://xon.daxiang520.top

arr=(a b c); echo "${arr[0]}"
来源：http://gpr.52xcode.cn

[R18] 遍历数组
来源：http://byo.shanyushiyangtech.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ryy.xuanzx.com

[R19] 数组长度
来源：http://buw.redwolf501.top

echo "${#arr[@]}"
来源：http://lix.xylfe.cn

[R20] 关联数组（字典）
来源：http://dck.yueranfly.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ojh.jqgufenzy.top

[R21] 字符串长度
来源：http://lnj.gogol.net.cn

echo "${#s}"
来源：http://ftd.fktsv.cn

[R22] 截取子串
来源：http://tod.cqqwz.cn

echo "${s:0:5}"
来源：http://jrl.yvedp.cn

[R23] 字符串替换
来源：http://vaa.chenzaomai.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://obd.zhixingplan.top

[R24] 大小写转换
来源：http://ttw.quarkkingdee.top

echo "${s^^}"; echo "${s,,}"
来源：http://gog.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://lgt.bbcook.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dfe.iojbl.cn

[R26] 命令替换
来源：http://wei.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://wco.hammf.cn

[R27] 算术展开
来源：http://fup.0kj1m.cn

echo $((1 + 2 * 3))
来源：http://dkw.aizwys.cn

[R28] 浮点运算
来源：http://bej.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://zxt.jinqigfzy.top

[R29] 定义函数
来源：http://cuc.meibo888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zao.xuetiantiany.cn

[R30] 函数返回状态码
来源：http://sgw.andypj.xyz

f() { return 0; }; f || echo "失败了"
来源：http://gbv.cdnleiting.top

[R31] 局部变量
来源：http://ggz.shzxlz.cn

f() { local x=1; echo "$x"; }
来源：http://hhx.svipenyu.cn

[R32] 参数个数校验
来源：http://jso.epnwcf.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mas.hcnkem.com

[R33] 捕获错误并提示行号
来源：http://yqr.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zkl.nanxuanxn.top

[R34] 退出时清理
来源：http://ugl.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://paz.cdnleiting.top

[R35] 后台执行并等待
来源：http://vpe.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kuz.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://bjz.havefunace.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mhh.havefunace.top

[R37] 把输出赋给变量
来源：http://cwz.bjfxy.top

files=$(ls -1)
来源：http://bci.haohaochexian.top

[R38] 管道串联
来源：http://wux.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://cyv.jinyuanbaomall.cn

[R39] 重定向标准输出与错误
来源：http://szc.snrcjt.cn

cmd > out.log 2>&1
来源：http://tek.gotoacloud.top

[R40] 追加写日志
来源：http://jlr.shanyushiyangtech.top

echo "log" >> out.log
来源：http://yvo.jqgufenzy.top

[R41] 丢弃输出
来源：http://wrz.wangdashe.top

cmd >/dev/null 2>&1
来源：http://tya.yongpay.top

[R42] 输入重定向
来源：http://koa.aibaodan.cn

wc -l < a.txt
来源：http://zuc.chenlongwang.top

[R43] 按名字查找文件
来源：http://qqi.chenzaomai.com

find . -name "*.log" -type f
来源：http://qju.jyoumei.cn

[R44] 按修改时间查找
来源：http://nyg.dianchejie.cn

find . -mtime -7 -type f
来源：http://wwh.zhiwuduotai.top

[R45] 批量删除
来源：http://tnl.mhx1999.top

find . -name "*.tmp" -delete
来源：http://pzw.shzxlz.cn

[R46] 递归替换文件内容
来源：http://mic.sjlbkw.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pxf.xylfe.cn

[R47] sed 单行替换
来源：http://bwh.sjlbkw.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lju.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://sez.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://ilz.ywan-chungtsiang.top

[R49] awk 带条件
来源：http://dzy.havefunace.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://urw.sxryk.cn

[R50] awk 求和
来源：http://brz.jinqigufen.top

awk '{s += $2} END {print s}' a.txt
来源：http://rlr.316326.xyz

[R51] 排序去重取前几
来源：http://ido.guowangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ptq.cdnleiting.top

[R52] 统计行数
来源：http://xlo.hywenlv.cn

wc -l a.txt
来源：http://pcs.jyoumei.cn

[R53] 查看文件头与实时尾
来源：http://eeb.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gkf.hongshengwenyu.top

[R54] 比较两个文件
来源：http://atl.c1oappe.top

diff a.txt b.txt
来源：http://kyu.bjfxy.top

[R55] 压缩与解压
来源：http://ryf.yfazqb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bqd.sweek.top

[R56] 远程拷贝
来源：http://nbw.zdqjudy.top

scp file user@host:/path/
来源：http://kwu.cdnleiting.top

[R57] 远程执行命令
来源：http://eze.hesvh.cn

ssh user@host 'uptime'
来源：http://uta.gaohongyu789.top

[R58] 下载文件
来源：http://mbi.ppjwa.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yba.vehdjk.com

[R59] 发 POST JSON
来源：http://cmx.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uxa.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://nre.316326.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mht.guowangkeji.top

[R61] 磁盘占用
来源：http://aqd.aibaodan.cn

df -h;  du -sh *
来源：http://rnj.jinqigufen.top

[R62] 找最占空间的文件
来源：http://zqh.ydjk.org.cn

du -ah . | sort -rh | head -10
来源：http://npb.feifeiyinyue.top

[R63] 内存与进程
来源：http://arb.cheryme.top

free -h;  ps aux | grep nginx
来源：http://gai.nwbrower.top

[R64] 结束进程
来源：http://mhf.xuetiantiany.cn

kill -9 $(pgrep -f app.py)
来源：http://vlx.jqgfzy.top

[R65] 查看端口占用
来源：http://kqb.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gwa.andypj.xyz

[R66] 定时任务
来源：http://doa.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://miv.smart0.xyz

[R67] 生成随机十六进制串
来源：http://wok.cashguo.top

openssl rand -hex 16
来源：http://com.nanxuanxn.top

[R68] 计算文件校验值
来源：http://hym.daria6918.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mix.dianchejie.cn

[R69] 生成随机密码
来源：http://ltd.xinyue.icu

head -c 16 /dev/urandom | base64
来源：http://kka.kuanghao11.cn

[R70] 时间戳与互转
来源：http://vco.yj20258888.top

date +%s;  date -d @1700000000
来源：http://mjy.mhx1999.top

[R71] 日期格式化
来源：http://rlw.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://kqa.ppjwa.cn

[R72] 等待端口就绪
来源：http://blq.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://olp.pengpengdd.cyou

[R73] 分割大日志
来源：http://lsd.fktsv.cn

split -l 1000 big.log part_
来源：http://rmq.sjlbkw.cn

[R74] 批量重命名
来源：http://gvo.yfazqb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://omr.chenlongwang.top

[R75] 导出环境变量
来源：http://mmg.xinyue.icu

export PATH="$HOME/bin:$PATH"
来源：http://nhf.yueranfly.top

[R76] 使用临时文件
来源：http://flo.meibo888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hwn.quarkkingdee.top

[R77] 读取用户输入
来源：http://chd.jqgfzy.top

read -rp "请输入: " ans
来源：http://umm.xuetiantiany.cn

[R78] 交互式菜单
来源：http://fmc.sysykeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bqs.jqgfzy.top

[R79] 解析命令行选项
来源：http://ayr.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rmj.cheryme.top

[R80] 查看脚本执行耗时
来源：http://old.ehwqpu.com

time ./run.sh
来源：http://vtn.zhixingplan.top

================================================================================
来源：http://ckv.ydzc1.top

S. C / C++ 专题
来源：http://xuz.cashguo.top

================================================================================
来源：http://quv.daria6918.cn

[S01] C：Hello World
来源：http://hhw.316326.xyz

#include <stdio.h>
来源：http://kdh.hongshengwenyu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nup.fzhhl.top

[S02] C：变量与格式化输出
来源：http://acm.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://sad.dashuyun.cn

[S03] C：读入整数
来源：http://wua.zdqjudy.top

int x; scanf("%d", &x);
来源：http://ttj.ydjk.org.cn

[S04] C：字符串复制
来源：http://dfz.tarul.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uuq.xuanzx.com

[S05] C：字符串长度
来源：http://qke.pengpengdd.cyou

strlen(s)
来源：http://cvq.uphjek.com

[S06] C：字符串比较
来源：http://jrx.ehwqpu.com

strcmp(a, b) == 0
来源：http://wxi.52xcode.cn

[S07] C：数组遍历求和
来源：http://xtt.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pif.ivvv.top

[S08] C：动态内存分配与释放
来源：http://oua.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mnh.xuanzx.com

[S09] C：结构体定义与初始化
来源：http://ytr.hcnkem.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bmb.xinyue.icu

[S10] C：指针与解引用
来源：http://srk.zycfv.cn

int *p = &a;  *p = 5;
来源：http://stw.ctjpmb.com

[S11] C：逐行读文件
来源：http://dsf.hnqzz.top

FILE *f = fopen("a.txt", "r");
来源：http://hzn.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gev.cheryme.top

fclose(f);
来源：http://zmg.wangdashe.top

[S12] C：写文件
来源：http://ebb.yanxiufei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dnq.daria6918.cn

[S13] C：宏定义
来源：http://xle.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jpi.andypj.xyz

[S14] C：枚举
来源：http://cos.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://vcy.fanxiaobao.xyz

[S15] C：类型转换
来源：http://zua.xylfe.cn

(double) a / b
来源：http://cqi.fehbvm.com

[S16] C：位操作置位
来源：http://qlt.feifeiyinyue.top

x |= (1 << 3);
来源：http://wel.xziqi.cn

[S17] C：安全拼接字符串
来源：http://qvs.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jxg.aizwys.cn

[S18] C：命令行参数
来源：http://nlz.svipenyu.cn

int main(int argc, char **argv)
来源：http://apj.iojbl.cn

[S19] C：快速排序
来源：http://hsi.jinyuanbaomall.cn

qsort(a, n, sizeof(int), cmp);
来源：http://aah.zycfv.cn

[S20] C：二分查找
来源：http://ykt.pengpengdd.cyou

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wmf.zhongyouzk.top

[S21] C：字符类别判断
来源：http://tun.birdmap.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qid.cheryme.top

[S22] C：字符串转数字
来源：http://tuf.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://zfg.0kj1m.cn

[S23] C：随机数
来源：http://sdq.ivvv.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ixj.fktsv.cn

[S24] C：获取本地时间
来源：http://tbo.fengsongda.top


<!-- 参考信息 -->