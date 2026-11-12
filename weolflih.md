代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jxl.jqgfzy.top

[Q54] 清空表
来源：http://nha.bjfxy.top

TRUNCATE TABLE logs;
来源：http://aqu.zhiwuduotai.top

[Q55] 排名（并列占位）
来源：http://ryp.sxryk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kjh.shanyushiyangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://cyb.dianchejie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wob.shanyushiyangkeji.top

[Q57] 行号
来源：http://dly.aibaodan.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tlg.meibo888.top

[Q58] 累计求和
来源：http://aix.cucudq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hvu.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://day.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://onx.vehdjk.com

[Q60] 取上一行 / 下一行
来源：http://drx.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xki.shanyushiyangtech.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://olw.yj20258.top

[Q61] 移动平均
来源：http://ggf.52xcode.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vei.0kj1m.cn

[Q62] 分组占比
来源：http://weu.svipenyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dyl.tanke756.top

[Q63] 开启事务
来源：http://bbk.fengsongda.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rrt.chenlongwang.top

[Q64] 提交事务
来源：http://tau.vehdjk.com

COMMIT;
来源：http://lfd.yueranfly.top

[Q65] 回滚事务
来源：http://fwq.hcnkem.com

ROLLBACK;
来源：http://mqu.feifeiyinyue.top

[Q66] 行锁查询
来源：http://nui.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wrt.wangdashe.top

[Q67] 设置隔离级别
来源：http://gsf.fzhhl.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kqg.tian-w.cn

[Q68] 保存点
来源：http://uvj.zhengqikj.top

SAVEPOINT sp1;
来源：http://mur.epnwcf.com

ROLLBACK TO sp1;
来源：http://biq.zhijiandao.cn

[Q69] 查看执行计划
来源：http://jiu.xingfuxueyuan.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xal.bjfxy.top

[Q70] 更新统计信息
来源：http://woa.quarkkingdee.top

ANALYZE TABLE users;
来源：http://ces.yj20258.top

[Q71] 查看建表语句
来源：http://way.jinghuilouyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fke.hywenlv.cn

[Q72] 查看索引
来源：http://imm.shuidangran.top

SHOW INDEX FROM users;
来源：http://cpa.316326.xyz

[Q73] 查看表状态
来源：http://ctz.kuanghao11.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yhw.guowangkeji.top

[Q74] 强制使用索引
来源：http://cex.meibo888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cmx.tarul.cn

[Q75] 日期格式化
来源：http://txa.wangshuangyany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tpy.svipenyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cnx.tian-w.cn

[Q76] 按天统计
来源：http://hye.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eva.chenlongwang.top

[Q77] 时间加减
来源：http://fkj.snrcjt.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cwp.jqgufenzy.top

[Q78] 当前时间
来源：http://eks.zycfv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pcb.epnwcf.com

[Q79] 字符串拼接
来源：http://qtm.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bwz.redwolf501.top

[Q80] 字符串截取
来源：http://tnq.jqgufenzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://inz.zhengqikj.top

[Q81] 字符串替换
来源：http://qbz.sufxvd.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zph.iojbl.cn

[Q82] 字符长度与字节长度
来源：http://wod.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nri.cqqwz.cn

[Q83] 大小写转换
来源：http://fmg.nanxinkj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jmh.yanxiufei.cn

[Q84] 去除首尾空格
来源：http://iwo.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://vow.9152youxi.cn

[Q85] 数值取整
来源：http://edc.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sqz.fehbvm.com

[Q86] 读取 JSON 字段
来源：http://qms.dashuyun.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zbe.xingfuxueyuan.xyz

[Q87] JSON 字段做条件
来源：http://meg.tianlin.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tnw.ivvv.top

[Q88] 行转列（条件聚合）
来源：http://exl.c1oappe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://usj.snrcjt.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uog.sxryk.cn

[Q89] 判断表是否存在
来源：http://ihd.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://haz.svipenyu.cn

[Q90] 生成序号列
来源：http://tns.chenjidiqi.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vqw.hammf.cn

================================================================================
来源：http://efh.jyoumei.cn

R. Bash 专题
来源：http://ppz.fktsv.cn

================================================================================
来源：http://dhm.yonumen.top

[R01] shebang 与严格模式
来源：http://jmv.dashuyun.cn

#!/usr/bin/env bash
来源：http://pgz.quarkkingdee.top

set -euo pipefail
来源：http://fru.redwolf501.top

[R02] 变量赋值与使用
来源：http://cvk.ivvv.top

name="Tom"; echo "$name"
来源：http://qkq.dashuyun.cn

[R03] 只读变量
来源：http://xwo.cucudq.cn

readonly PI=3.14
来源：http://xdj.zhixingplan.top

[R04] 位置参数
来源：http://jjh.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yqp.guowangkeji.top

[R05] 参数默认值
来源：http://pex.shzxlz.cn

name="${1:-default}"
来源：http://czw.fktsv.cn

[R06] 判断命令是否存在
来源：http://ngr.nwbrower.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vpo.aizwys.cn

[R07] if 判断文件
来源：http://ymi.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rqa.sysykeji.top

[R08] 数值比较
来源：http://cwn.gaohongyu789.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fkl.jqgufenzy.top

[R09] 字符串比较
来源：http://njv.andypj.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ffu.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://eab.jqgufenzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://atd.yj20258888.top

[R11] case 多分支
来源：http://gvq.yuxming.cn

case "$1" in
来源：http://ayx.xuanzx.com

start) echo "启动" ;;
来源：http://kgb.bbcook.cn

stop)  echo "停止" ;;
来源：http://mlz.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://onu.smart0.xyz

esac
来源：http://lir.fzhhl.top

[R12] for 遍历文件
来源：http://dcx.guowangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://rty.yj20258.top

[R13] for 计数循环
来源：http://nbh.ctjpmb.com

for i in {1..10}; do echo "$i"; done
来源：http://vkx.haohaochexian.top

[R14] C 风格 for
来源：http://jhg.sxryk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bho.ehwqpu.com

[R15] while 逐行读文件
来源：http://cqh.uphjek.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bqa.ivvv.top

[R16] until 等待条件
来源：http://wdz.xziqi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hdv.zdbjq.cn

[R17] 数组定义与取值
来源：http://vog.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://afh.ppjwa.cn

[R18] 遍历数组
来源：http://xck.fehbvm.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vqx.vehdjk.com

[R19] 数组长度
来源：http://sdk.wangshuangyany.cn

echo "${#arr[@]}"
来源：http://vkk.zhoulong.xyz

[R20] 关联数组（字典）
来源：http://ibv.hnqzz.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qkr.jinqigfzy.top

[R21] 字符串长度
来源：http://pvj.yj20258.top

echo "${#s}"
来源：http://moz.yanxiufei.cn

[R22] 截取子串
来源：http://ezx.haohaochexian.top

echo "${s:0:5}"
来源：http://wfk.chenjidiqi.icu

[R23] 字符串替换
来源：http://bkf.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://knd.cdnleiting.top

[R24] 大小写转换
来源：http://fhi.zhaomingkeji.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://gxc.jqgufenzy.top

[R25] 去后缀 / 去前缀
来源：http://tkp.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dal.hfpthk.cn

[R26] 命令替换
来源：http://kvv.yj202588.top

now=$(date +%F); echo "$now"
来源：http://qca.bbcook.cn

[R27] 算术展开
来源：http://xcc.fzhhl.top

echo $((1 + 2 * 3))
来源：http://dtq.uphjek.com

[R28] 浮点运算
来源：http://unv.dashuyun.cn

echo "scale=2; 10/3" | bc
来源：http://wgu.vehdjk.com

[R29] 定义函数
来源：http://iwm.cheryme.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iqo.dianchejie.cn

[R30] 函数返回状态码
来源：http://ioo.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://uxj.xziqi.cn

[R31] 局部变量
来源：http://xvr.bbcook.cn

f() { local x=1; echo "$x"; }
来源：http://wgi.zdbjq.cn

[R32] 参数个数校验
来源：http://nvs.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://frx.tarul.cn

[R33] 捕获错误并提示行号
来源：http://hba.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://omo.hfpthk.cn

[R34] 退出时清理
来源：http://lxf.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bos.hammf.cn

[R35] 后台执行并等待
来源：http://fnm.dianchejie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mex.jiagoushi.top

[R36] 并发执行多个任务
来源：http://shi.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zfh.gzhubu.top

[R37] 把输出赋给变量
来源：http://kpp.gogol.net.cn

files=$(ls -1)
来源：http://fvm.yangfankeji.com

[R38] 管道串联
来源：http://koo.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://eye.snrcjt.cn

[R39] 重定向标准输出与错误
来源：http://acy.yj20258.top

cmd > out.log 2>&1
来源：http://qjg.sxryk.cn

[R40] 追加写日志
来源：http://avf.sxryk.cn

echo "log" >> out.log
来源：http://zwn.fehbvm.com

[R41] 丢弃输出
来源：http://uys.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://kzr.chenjidiqi.icu

[R42] 输入重定向
来源：http://kmf.yj202588.top

wc -l < a.txt
来源：http://mrn.smart0.xyz

[R43] 按名字查找文件
来源：http://ryw.0kj1m.cn

find . -name "*.log" -type f
来源：http://uca.jyoumei.cn

[R44] 按修改时间查找
来源：http://rhx.pycfn.com

find . -mtime -7 -type f
来源：http://fqs.ctjpmb.com

[R45] 批量删除
来源：http://gpm.zhengqikj.top

find . -name "*.tmp" -delete
来源：http://nkb.jianghu66.top

[R46] 递归替换文件内容
来源：http://ylr.mhx1999.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mqz.sxryk.cn

[R47] sed 单行替换
来源：http://mmj.feifeiyinyue.top

sed -i 's/foo/bar/g' a.txt
来源：http://oym.hysaishi.cn

[R48] awk 取指定列
来源：http://kxa.tarul.cn

awk '{print $1, $3}' a.txt
来源：http://axr.havefunace.top

[R49] awk 带条件
来源：http://cfg.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://emy.xuetiantiany.cn

[R50] awk 求和
来源：http://fgn.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://qfv.sysykeji.top

[R51] 排序去重取前几
来源：http://rwt.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yep.jinghuilouyu.cn

[R52] 统计行数
来源：http://var.redwolf501.top

wc -l a.txt
来源：http://mqc.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://wsc.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lvl.yj20258888.top

[R54] 比较两个文件
来源：http://ont.zhoulong.xyz

diff a.txt b.txt
来源：http://qtm.xingfuxueyuan.xyz

[R55] 压缩与解压
来源：http://svu.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gfn.yj20258888.top

[R56] 远程拷贝
来源：http://zwn.mhx1999.top

scp file user@host:/path/
来源：http://lto.zycfv.cn

[R57] 远程执行命令
来源：http://jvz.zhaomingkeji.xyz

ssh user@host 'uptime'
来源：http://voz.316326.xyz

[R58] 下载文件
来源：http://gqx.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gom.hcnkem.com

[R59] 发 POST JSON
来源：http://hoi.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ttb.daxiang520.top

[R60] 只看 HTTP 状态码
来源：http://srj.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nsi.yueranfly.top

[R61] 磁盘占用
来源：http://owv.quarkkingdee.top

df -h;  du -sh *
来源：http://cfc.yvedp.cn

[R62] 找最占空间的文件
来源：http://ilu.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://zme.kuanghao11.cn

[R63] 内存与进程
来源：http://upa.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://bal.cheryme.top

[R64] 结束进程
来源：http://dbt.yj20258888.top

kill -9 $(pgrep -f app.py)
来源：http://dmg.zhoulong.xyz

[R65] 查看端口占用
来源：http://tse.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cdt.chenzaomai.com

[R66] 定时任务
来源：http://sht.jqgfzy.top

crontab -e;  crontab -l
来源：http://vdr.tianlin.xyz

[R67] 生成随机十六进制串
来源：http://iui.haohaochexian.top

openssl rand -hex 16
来源：http://aag.xuanzx.com

[R68] 计算文件校验值
来源：http://pxw.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://axz.ydzc1.top

[R69] 生成随机密码
来源：http://afc.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://mri.hfpthk.cn

[R70] 时间戳与互转
来源：http://ise.cheryme.top

date +%s;  date -d @1700000000
来源：http://xwc.jinyuanbaomall.cn

[R71] 日期格式化
来源：http://euj.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pdg.bbcook.cn

[R72] 等待端口就绪
来源：http://ydt.dianchejie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jxi.yanxiufei.cn

[R73] 分割大日志
来源：http://jnj.ydjk.org.cn

split -l 1000 big.log part_
来源：http://azu.cucudq.cn

[R74] 批量重命名
来源：http://cjz.cqqwz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lar.jiagoushi.top

[R75] 导出环境变量
来源：http://ldt.yongpay.top

export PATH="$HOME/bin:$PATH"
来源：http://kra.cucudq.cn

[R76] 使用临时文件
来源：http://grj.epnwcf.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bpn.nwbrower.top

[R77] 读取用户输入
来源：http://jfh.haohaochexian.top

read -rp "请输入: " ans
来源：http://dti.havefunace.top

[R78] 交互式菜单
来源：http://ngl.ydzc1.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wrl.nanxuanxn.top

[R79] 解析命令行选项
来源：http://cuh.xylfe.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mng.yonumen.top

[R80] 查看脚本执行耗时
来源：http://lly.jinyuanbaomall.cn

time ./run.sh
来源：http://rkx.quarkkingdee.top

================================================================================
来源：http://zoz.shanyushiyangtech.top

S. C / C++ 专题
来源：http://jzf.havefunace.top

================================================================================
来源：http://tsp.ivvv.top

[S01] C：Hello World
来源：http://qpu.gaohongyu789.top

#include <stdio.h>
来源：http://ept.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://apo.zhixingplan.top

[S02] C：变量与格式化输出
来源：http://ahx.xziqi.cn

int a = 10; printf("%d\n", a);
来源：http://iuy.cashguo.top

[S03] C：读入整数
来源：http://qyf.ivvv.top

int x; scanf("%d", &x);
来源：http://zal.meibo888.top

[S04] C：字符串复制
来源：http://ccc.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://fza.316326.xyz

[S05] C：字符串长度
来源：http://hjf.chenzaomai.com

strlen(s)
来源：http://rky.nanxuanxn.top

[S06] C：字符串比较
来源：http://rqn.dianchejie.cn

strcmp(a, b) == 0
来源：http://wdd.kuanghao11.cn

[S07] C：数组遍历求和
来源：http://wez.sweek.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://udh.9152youxi.cn

[S08] C：动态内存分配与释放
来源：http://xcw.hesvh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gif.feifeiyinyue.top

[S09] C：结构体定义与初始化
来源：http://lvs.fengsongda.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cli.tarul.cn

[S10] C：指针与解引用
来源：http://ezc.yj20258.top

int *p = &a;  *p = 5;
来源：http://nmn.hywenlv.cn

[S11] C：逐行读文件
来源：http://kqg.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://fnw.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rsp.bjfxy.top

fclose(f);
来源：http://wmp.svipenyu.cn

[S12] C：写文件
来源：http://qaf.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://euc.xinyue.icu

[S13] C：宏定义
来源：http://mzy.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vne.ydjk.org.cn

[S14] C：枚举
来源：http://uwu.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://gfh.andypj.xyz

[S15] C：类型转换
来源：http://bue.yongpay.top

(double) a / b
来源：http://ywm.jianghu66.top

[S16] C：位操作置位
来源：http://cqs.9152youxi.cn

x |= (1 << 3);
来源：http://poc.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://baf.zycfv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jyu.tarul.cn

[S18] C：命令行参数
来源：http://bmm.quarkkingdee.top

int main(int argc, char **argv)
来源：http://lsf.gogol.net.cn

[S19] C：快速排序
来源：http://kfr.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://ewm.gaohongyu789.top

[S20] C：二分查找
来源：http://hbv.andypj.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ljc.fktsv.cn

[S21] C：字符类别判断
来源：http://tyg.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://epb.shzxlz.cn

[S22] C：字符串转数字
来源：http://fgv.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://agl.uphjek.com

[S23] C：随机数
来源：http://qvc.yvedp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mxg.hnqzz.top

[S24] C：获取本地时间
来源：http://yjo.ybcxt.top


<!-- 参考信息 -->