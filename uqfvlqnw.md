代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ycz.xziqi.cn

[Q56] 密集排名（并列不占位）
来源：http://oxr.fanxiaobao.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://plh.hnxiangtu.top

[Q57] 行号
来源：http://hbj.zdqjudy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dke.yvedp.cn

[Q58] 累计求和
来源：http://ouv.iojbl.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yyq.sjlbkw.cn

[Q59] 分组内累计
来源：http://phw.sweek.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ryj.yanxiufei.cn

[Q60] 取上一行 / 下一行
来源：http://mmz.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rmo.cashguo.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pmx.nwbrower.top

[Q61] 移动平均
来源：http://xsm.zdqjudy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xpu.wangshuangyany.cn

[Q62] 分组占比
来源：http://jxf.quarkkingdee.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zud.zhengqikj.top

[Q63] 开启事务
来源：http://bvf.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ruv.fehbvm.com

[Q64] 提交事务
来源：http://oek.hfpthk.cn

COMMIT;
来源：http://crd.hfpthk.cn

[Q65] 回滚事务
来源：http://bbo.ydjk.org.cn

ROLLBACK;
来源：http://npw.hesvh.cn

[Q66] 行锁查询
来源：http://xnf.shanyushiyangtech.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gky.zhengqikj.top

[Q67] 设置隔离级别
来源：http://akg.zhongyouzk.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bsi.tarul.cn

[Q68] 保存点
来源：http://gbg.ydjk.org.cn

SAVEPOINT sp1;
来源：http://kjx.bbcook.cn

ROLLBACK TO sp1;
来源：http://ght.dianchejie.cn

[Q69] 查看执行计划
来源：http://ptx.yangfankeji.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qit.feifeiyinyue.top

[Q70] 更新统计信息
来源：http://xxv.birdmap.top

ANALYZE TABLE users;
来源：http://nyy.chenzaomai.com

[Q71] 查看建表语句
来源：http://qmg.gogol.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pvw.dianchejie.cn

[Q72] 查看索引
来源：http://jnk.havefunace.top

SHOW INDEX FROM users;
来源：http://ptc.hcnkem.com

[Q73] 查看表状态
来源：http://kvc.zhengqikj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zcf.birdmap.top

[Q74] 强制使用索引
来源：http://uah.zhixingplan.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hrn.zhiwuduotai.top

[Q75] 日期格式化
来源：http://qeb.aizwys.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mlo.tian-w.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rwh.uphjek.com

[Q76] 按天统计
来源：http://hur.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://odg.hesvh.cn

[Q77] 时间加减
来源：http://dpb.cqqwz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rxz.wangdashe.top

[Q78] 当前时间
来源：http://lun.gzhubu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pso.kuanghao11.cn

[Q79] 字符串拼接
来源：http://mqh.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mhi.cheryme.top

[Q80] 字符串截取
来源：http://klk.fktsv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xbq.jlsjyb.cn

[Q81] 字符串替换
来源：http://nxd.gaohongyu789.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://eep.gogol.net.cn

[Q82] 字符长度与字节长度
来源：http://gjt.cucudq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rju.chenlongwang.top

[Q83] 大小写转换
来源：http://dnt.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jkw.zycfv.cn

[Q84] 去除首尾空格
来源：http://zin.xuanzx.com

SELECT TRIM(name) FROM users;
来源：http://xdb.yuanzhike.top

[Q85] 数值取整
来源：http://hza.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yui.tianlin.xyz

[Q86] 读取 JSON 字段
来源：http://cuj.zhixingplan.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gnv.hnqzz.top

[Q87] JSON 字段做条件
来源：http://ufv.xuetiantiany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mcw.cqqwz.cn

[Q88] 行转列（条件聚合）
来源：http://bmu.yvedp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://noq.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://snz.sxryk.cn

[Q89] 判断表是否存在
来源：http://pjj.xziqi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mwf.hnxiangtu.top

[Q90] 生成序号列
来源：http://zsy.zycfv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zje.zdqjudy.top

================================================================================
来源：http://ofp.jqgufenzy.top

R. Bash 专题
来源：http://omg.zhoulong.xyz

================================================================================
来源：http://gvy.feifeiyinyue.top

[R01] shebang 与严格模式
来源：http://jhq.hongshengwenyu.top

#!/usr/bin/env bash
来源：http://ubv.cashguo.top

set -euo pipefail
来源：http://vnm.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://usu.ydzc1.top

name="Tom"; echo "$name"
来源：http://bla.nwbrower.top

[R03] 只读变量
来源：http://pud.havefunace.top

readonly PI=3.14
来源：http://fmu.shangyingyoupin.top

[R04] 位置参数
来源：http://qnr.316326.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ojp.epnwcf.com

[R05] 参数默认值
来源：http://vos.ybcxt.top

name="${1:-default}"
来源：http://bcs.sxryk.cn

[R06] 判断命令是否存在
来源：http://ryi.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ujv.yangfankeji.com

[R07] if 判断文件
来源：http://iqd.daria6918.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vzm.hcnkem.com

[R08] 数值比较
来源：http://fxr.chenjidiqi.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://vff.kuanghao11.cn

[R09] 字符串比较
来源：http://szj.cdnleiting.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xye.vqdsnc.cn

[R10] 正则匹配
来源：http://bmp.sjlbkw.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uem.zdqjudy.top

[R11] case 多分支
来源：http://gcm.tarul.cn

case "$1" in
来源：http://ysz.aibaodan.cn

start) echo "启动" ;;
来源：http://pjh.fktsv.cn

stop)  echo "停止" ;;
来源：http://olb.xuanzx.com

*)     echo "未知命令" ;;
来源：http://tun.hfpthk.cn

esac
来源：http://wja.zhijiandao.cn

[R12] for 遍历文件
来源：http://noj.ydzc1.top

for f in *.txt; do echo "$f"; done
来源：http://rxs.ehwqpu.com

[R13] for 计数循环
来源：http://vro.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://fzm.yueranfly.top

[R14] C 风格 for
来源：http://sfg.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qck.hcnkem.com

[R15] while 逐行读文件
来源：http://fkl.nwbrower.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vev.tarul.cn

[R16] until 等待条件
来源：http://tyg.ywan-chungtsiang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://prf.jinqigfzy.top

[R17] 数组定义与取值
来源：http://jpl.sjlbkw.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jzh.52xcode.cn

[R18] 遍历数组
来源：http://fta.jyoumei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://slm.chenjidiqi.icu

[R19] 数组长度
来源：http://yvr.meibo888.top

echo "${#arr[@]}"
来源：http://itz.daxiang520.top

[R20] 关联数组（字典）
来源：http://ayg.jlsjyb.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tfu.yvedp.cn

[R21] 字符串长度
来源：http://blq.chenlongwang.top

echo "${#s}"
来源：http://nie.sweek.top

[R22] 截取子串
来源：http://trx.zhongyouzk.top

echo "${s:0:5}"
来源：http://zhh.jyoumei.cn

[R23] 字符串替换
来源：http://whs.ehwqpu.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nuc.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://bvy.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ttx.iojbl.cn

[R25] 去后缀 / 去前缀
来源：http://jqg.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uvi.pengpengdd.cyou

[R26] 命令替换
来源：http://szl.vqdsnc.cn

now=$(date +%F); echo "$now"
来源：http://mjc.yanxiufei.cn

[R27] 算术展开
来源：http://twi.xziqi.cn

echo $((1 + 2 * 3))
来源：http://jin.jyoumei.cn

[R28] 浮点运算
来源：http://xix.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://vip.jiagoushi.top

[R29] 定义函数
来源：http://fyn.ywan-chungtsiang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cal.nanxinkj.top

[R30] 函数返回状态码
来源：http://ovi.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://qif.hammf.cn

[R31] 局部变量
来源：http://zzd.jlsjyb.cn

f() { local x=1; echo "$x"; }
来源：http://uib.jianghu66.top

[R32] 参数个数校验
来源：http://wyo.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cbw.fzhhl.top

[R33] 捕获错误并提示行号
来源：http://ytg.hongshengwenyu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://enf.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://xhw.gaohongyu789.top

trap 'rm -f "$tmp"' EXIT
来源：http://siq.sweek.top

[R35] 后台执行并等待
来源：http://soy.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gvd.9152youxi.cn

[R36] 并发执行多个任务
来源：http://tkb.wangdashe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://grl.hysaishi.cn

[R37] 把输出赋给变量
来源：http://ksl.smart0.xyz

files=$(ls -1)
来源：http://kvb.guowangkeji.top

[R38] 管道串联
来源：http://ayl.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://yqm.epnwcf.com

[R39] 重定向标准输出与错误
来源：http://asa.yuxming.cn

cmd > out.log 2>&1
来源：http://jzf.yvedp.cn

[R40] 追加写日志
来源：http://mce.gaohongyu789.top

echo "log" >> out.log
来源：http://vtu.yueranfly.top

[R41] 丢弃输出
来源：http://tkw.xziqi.cn

cmd >/dev/null 2>&1
来源：http://bdv.9152youxi.cn

[R42] 输入重定向
来源：http://des.sufxvd.cn

wc -l < a.txt
来源：http://pyi.pengpengdd.cyou

[R43] 按名字查找文件
来源：http://ocs.ydjk.org.cn

find . -name "*.log" -type f
来源：http://vmg.aibaodan.cn

[R44] 按修改时间查找
来源：http://obn.jiagoushi.top

find . -mtime -7 -type f
来源：http://ump.fehbvm.com

[R45] 批量删除
来源：http://laf.yvedp.cn

find . -name "*.tmp" -delete
来源：http://pgb.bbcook.cn

[R46] 递归替换文件内容
来源：http://kwh.jqgfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jnb.andypj.xyz

[R47] sed 单行替换
来源：http://uew.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fjd.hammf.cn

[R48] awk 取指定列
来源：http://dff.jianghu66.top

awk '{print $1, $3}' a.txt
来源：http://xhg.jiagoushi.top

[R49] awk 带条件
来源：http://uat.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bqf.zhaomingkeji.xyz

[R50] awk 求和
来源：http://oyt.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lmp.cdnleiting.top

[R51] 排序去重取前几
来源：http://wkp.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://eyh.yonumen.top

[R52] 统计行数
来源：http://qlt.guowangkeji.top

wc -l a.txt
来源：http://bgg.hnqzz.top

[R53] 查看文件头与实时尾
来源：http://yqu.jinqigufen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wox.nanxinkj.top

[R54] 比较两个文件
来源：http://xjq.ydzc1.top

diff a.txt b.txt
来源：http://usq.cashguo.top

[R55] 压缩与解压
来源：http://fvn.9152youxi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bnp.ppjwa.cn

[R56] 远程拷贝
来源：http://nsg.bjfxy.top

scp file user@host:/path/
来源：http://ssd.sjlbkw.cn

[R57] 远程执行命令
来源：http://pog.hongshengwenyu.top

ssh user@host 'uptime'
来源：http://csx.hongshengwenyu.top

[R58] 下载文件
来源：http://cvk.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mto.birdmap.top

[R59] 发 POST JSON
来源：http://ahe.zhoulong.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vxx.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://ykd.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rye.chenlongwang.top

[R61] 磁盘占用
来源：http://xpz.tanke756.top

df -h;  du -sh *
来源：http://qyo.yonumen.top

[R62] 找最占空间的文件
来源：http://heg.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://nsq.jinqigufen.top

[R63] 内存与进程
来源：http://wzu.c1oappe.top

free -h;  ps aux | grep nginx
来源：http://jjt.0kj1m.cn

[R64] 结束进程
来源：http://qrh.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://qxe.jinqigfzy.top

[R65] 查看端口占用
来源：http://fiu.316326.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zbh.pengpengdd.cyou

[R66] 定时任务
来源：http://sot.uphjek.com

crontab -e;  crontab -l
来源：http://gso.hfpthk.cn

[R67] 生成随机十六进制串
来源：http://cpf.nwbrower.top

openssl rand -hex 16
来源：http://huu.shuidangran.top

[R68] 计算文件校验值
来源：http://ame.nanxinkj.top

sha256sum a.txt;  md5sum a.txt
来源：http://qpa.xuetiantiany.cn

[R69] 生成随机密码
来源：http://qud.gaohongyu789.top

head -c 16 /dev/urandom | base64
来源：http://awb.haohaochexian.top

[R70] 时间戳与互转
来源：http://gue.pycfn.com

date +%s;  date -d @1700000000
来源：http://twa.ppjwa.cn

[R71] 日期格式化
来源：http://kpn.snrcjt.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bae.xuanzx.com

[R72] 等待端口就绪
来源：http://hcp.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://rab.dashuyun.cn

[R73] 分割大日志
来源：http://xfz.cheryme.top

split -l 1000 big.log part_
来源：http://bhk.jianghu66.top

[R74] 批量重命名
来源：http://zaf.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jhs.guowangkeji.top

[R75] 导出环境变量
来源：http://tum.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://bqm.zhaomingkeji.xyz

[R76] 使用临时文件
来源：http://jrg.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ukj.snrcjt.cn

[R77] 读取用户输入
来源：http://mvs.yueranfly.top

read -rp "请输入: " ans
来源：http://wha.zhoulong.xyz

[R78] 交互式菜单
来源：http://luh.xylfe.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gte.fengsongda.top

[R79] 解析命令行选项
来源：http://usm.jinqigufen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ogu.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://fta.guowangkeji.top

time ./run.sh
来源：http://wqm.quarkkingdee.top

================================================================================
来源：http://ubb.gaohongyu789.top

S. C / C++ 专题
来源：http://ine.xylfe.cn

================================================================================
来源：http://mzf.yueranfly.top

[S01] C：Hello World
来源：http://rod.yueranfly.top

#include <stdio.h>
来源：http://gfq.nwbrower.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rsh.cashguo.top

[S02] C：变量与格式化输出
来源：http://qrs.jinghuilouyu.cn

int a = 10; printf("%d\n", a);
来源：http://dom.cashguo.top

[S03] C：读入整数
来源：http://vug.yangfankeji.com

int x; scanf("%d", &x);
来源：http://ikk.hesvh.cn

[S04] C：字符串复制
来源：http://qup.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://ehw.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://ptj.guowangkeji.top

strlen(s)
来源：http://qpi.cucudq.cn

[S06] C：字符串比较
来源：http://drz.gogol.net.cn

strcmp(a, b) == 0
来源：http://bux.sxryk.cn

[S07] C：数组遍历求和
来源：http://dmu.yanxiufei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bsf.gogol.net.cn

[S08] C：动态内存分配与释放
来源：http://uij.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yla.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://omh.daria6918.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zkp.tianlin.xyz

[S10] C：指针与解引用
来源：http://wqa.yanxiufei.cn

int *p = &a;  *p = 5;
来源：http://krj.ydzc1.top

[S11] C：逐行读文件
来源：http://leh.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://hbf.dianchejie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lyj.fanxiaobao.xyz

fclose(f);
来源：http://auj.ywan-chungtsiang.top

[S12] C：写文件
来源：http://rgt.0kj1m.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://exy.pengpengdd.cyou

[S13] C：宏定义
来源：http://ekp.shuidangran.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xdx.bbcook.cn

[S14] C：枚举
来源：http://abn.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://fhy.wangshuangyany.cn

[S15] C：类型转换
来源：http://mpj.ydzc1.top

(double) a / b
来源：http://qxr.feifeiyinyue.top

[S16] C：位操作置位
来源：http://avy.gogol.net.cn

x |= (1 << 3);
来源：http://yyc.tanke756.top

[S17] C：安全拼接字符串
来源：http://pzu.shuidangran.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wup.ivvv.top

[S18] C：命令行参数
来源：http://jpc.vqdsnc.cn

int main(int argc, char **argv)
来源：http://chz.hysaishi.cn

[S19] C：快速排序
来源：http://fft.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cuh.hcnkem.com

[S20] C：二分查找
来源：http://aiv.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eom.nanxinkj.top

[S21] C：字符类别判断
来源：http://yuf.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ron.bbcook.cn

[S22] C：字符串转数字
来源：http://opi.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://alq.zycfv.cn

[S23] C：随机数
来源：http://zwe.sysykeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rxf.tian-w.cn

[S24] C：获取本地时间
来源：http://ydj.jiagoushi.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ruk.shuidangran.top

[S25] C：内存拷贝
来源：http://dwt.shuidangran.top

memcpy(dst, src, n);
来源：http://irz.nwbrower.top

[S26] C：内存清零
来源：http://fyf.gaohongyu789.top


<!-- 参考信息 -->