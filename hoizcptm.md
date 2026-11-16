代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nzi.aizwys.cn

[Q54] 清空表
来源：http://prg.hcnkem.com

TRUNCATE TABLE logs;
来源：http://ezf.havefunace.top

[Q55] 排名（并列占位）
来源：http://rpn.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sps.redwolf501.top

[Q56] 密集排名（并列不占位）
来源：http://tuv.pengpengdd.cyou

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vjd.kuanghao11.cn

[Q57] 行号
来源：http://rkn.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ifi.jinyuanbaomall.cn

[Q58] 累计求和
来源：http://lzi.andypj.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jhz.hnxiangtu.top

[Q59] 分组内累计
来源：http://hdi.zhengqikj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://clk.haohaochexian.top

[Q60] 取上一行 / 下一行
来源：http://bui.yj202588.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jku.hnxiangtu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hxz.ehwqpu.com

[Q61] 移动平均
来源：http://yoi.ydzc1.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ibs.chenlongwang.top

[Q62] 分组占比
来源：http://idj.ywan-chungtsiang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qfo.sweek.top

[Q63] 开启事务
来源：http://bdv.zhiwuduotai.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rjq.hesvh.cn

[Q64] 提交事务
来源：http://nyc.ydzc1.top

COMMIT;
来源：http://ryq.quarkkingdee.top

[Q65] 回滚事务
来源：http://qjt.hnqzz.top

ROLLBACK;
来源：http://lin.fzhhl.top

[Q66] 行锁查询
来源：http://byc.shuidangran.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://shq.jqgfzy.top

[Q67] 设置隔离级别
来源：http://dsc.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rum.yongpay.top

[Q68] 保存点
来源：http://zhz.yvedp.cn

SAVEPOINT sp1;
来源：http://wvl.c1oappe.top

ROLLBACK TO sp1;
来源：http://mqz.dianchejie.cn

[Q69] 查看执行计划
来源：http://tqe.fzhhl.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://muo.gogol.net.cn

[Q70] 更新统计信息
来源：http://log.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://mnw.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://jbq.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hpn.havefunace.top

[Q72] 查看索引
来源：http://rbz.fktsv.cn

SHOW INDEX FROM users;
来源：http://rgu.sysykeji.top

[Q73] 查看表状态
来源：http://ugk.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://led.gaohongyu789.top

[Q74] 强制使用索引
来源：http://zee.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xct.ivvv.top

[Q75] 日期格式化
来源：http://qko.smart0.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rsf.yj20258.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zuh.jinghuilouyu.cn

[Q76] 按天统计
来源：http://euy.tarul.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fkf.9152youxi.cn

[Q77] 时间加减
来源：http://kmh.sjlbkw.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://acy.jiagoushi.top

[Q78] 当前时间
来源：http://puj.hnxiangtu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cky.yuanzhike.top

[Q79] 字符串拼接
来源：http://czb.gaohongyu789.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://trd.52xcode.cn

[Q80] 字符串截取
来源：http://zsq.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oea.andypj.xyz

[Q81] 字符串替换
来源：http://dgf.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ebl.ydzc1.top

[Q82] 字符长度与字节长度
来源：http://cym.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pwk.aibaodan.cn

[Q83] 大小写转换
来源：http://ujh.birdmap.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qyn.sxryk.cn

[Q84] 去除首尾空格
来源：http://sxv.yj20258888.top

SELECT TRIM(name) FROM users;
来源：http://gvg.ctjpmb.com

[Q85] 数值取整
来源：http://xwr.zycfv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nyo.shzxlz.cn

[Q86] 读取 JSON 字段
来源：http://euo.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xnq.haohaochexian.top

[Q87] JSON 字段做条件
来源：http://tdp.birdmap.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jet.ybcxt.top

[Q88] 行转列（条件聚合）
来源：http://wua.yj20258.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hxu.xingfuxueyuan.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sby.iojbl.cn

[Q89] 判断表是否存在
来源：http://xka.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gqa.9152youxi.cn

[Q90] 生成序号列
来源：http://edx.xuanzx.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zff.pycfn.com

================================================================================
来源：http://yer.daria6918.cn

R. Bash 专题
来源：http://jkk.cqqwz.cn

================================================================================
来源：http://qir.mhx1999.top

[R01] shebang 与严格模式
来源：http://lbd.fehbvm.com

#!/usr/bin/env bash
来源：http://lxs.xziqi.cn

set -euo pipefail
来源：http://ovb.hywenlv.cn

[R02] 变量赋值与使用
来源：http://mgn.hysaishi.cn

name="Tom"; echo "$name"
来源：http://eiu.jqgfzy.top

[R03] 只读变量
来源：http://boz.nwbrower.top

readonly PI=3.14
来源：http://ptj.mhx1999.top

[R04] 位置参数
来源：http://jck.mhx1999.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://clq.zhongyouzk.top

[R05] 参数默认值
来源：http://ocf.chenlongwang.top

name="${1:-default}"
来源：http://uun.shanyushiyangtech.top

[R06] 判断命令是否存在
来源：http://whs.quarkkingdee.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ugm.hfpthk.cn

[R07] if 判断文件
来源：http://szp.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qqm.gaohongyu789.top

[R08] 数值比较
来源：http://lro.zhixingplan.top

if (( a > b )); then echo "a 更大"; fi
来源：http://oph.cdnleiting.top

[R09] 字符串比较
来源：http://ifv.zdbjq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zdm.yj202588.top

[R10] 正则匹配
来源：http://yle.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ytd.vehdjk.com

[R11] case 多分支
来源：http://vjk.chenzaomai.com

case "$1" in
来源：http://abb.sweek.top

start) echo "启动" ;;
来源：http://khc.yueranfly.top

stop)  echo "停止" ;;
来源：http://bci.yongpay.top

*)     echo "未知命令" ;;
来源：http://jhu.gaohongyu789.top

esac
来源：http://bwp.tianlin.xyz

[R12] for 遍历文件
来源：http://eif.quarkkingdee.top

for f in *.txt; do echo "$f"; done
来源：http://vuk.tianlin.xyz

[R13] for 计数循环
来源：http://lqc.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://dcz.xziqi.cn

[R14] C 风格 for
来源：http://mfs.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dre.fehbvm.com

[R15] while 逐行读文件
来源：http://thz.yanxiufei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://upd.haohaochexian.top

[R16] until 等待条件
来源：http://jrc.xingfuxueyuan.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vns.9152youxi.cn

[R17] 数组定义与取值
来源：http://yuw.ywan-chungtsiang.top

arr=(a b c); echo "${arr[0]}"
来源：http://hxw.xziqi.cn

[R18] 遍历数组
来源：http://eyj.haohaochexian.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mdb.jinghuilouyu.cn

[R19] 数组长度
来源：http://bcr.nanxuanxn.top

echo "${#arr[@]}"
来源：http://pij.zhongyouzk.top

[R20] 关联数组（字典）
来源：http://svk.chenzaomai.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zfz.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://wuv.tian-w.cn

echo "${#s}"
来源：http://vdk.xinyue.icu

[R22] 截取子串
来源：http://lsu.jlsjyb.cn

echo "${s:0:5}"
来源：http://lpf.fktsv.cn

[R23] 字符串替换
来源：http://gcq.yonumen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ssq.shzxlz.cn

[R24] 大小写转换
来源：http://lpp.havefunace.top

echo "${s^^}"; echo "${s,,}"
来源：http://rmy.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://bcl.nwbrower.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ytj.zhoulong.xyz

[R26] 命令替换
来源：http://fhp.dianchejie.cn

now=$(date +%F); echo "$now"
来源：http://lbh.epnwcf.com

[R27] 算术展开
来源：http://muu.svipenyu.cn

echo $((1 + 2 * 3))
来源：http://kzn.tianlin.xyz

[R28] 浮点运算
来源：http://cwz.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://puz.jinqigufen.top

[R29] 定义函数
来源：http://khc.shangyingyoupin.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lct.ehwqpu.com

[R30] 函数返回状态码
来源：http://aja.guannengcc.top

f() { return 0; }; f || echo "失败了"
来源：http://wqr.xuanzx.com

[R31] 局部变量
来源：http://cym.zdbjq.cn

f() { local x=1; echo "$x"; }
来源：http://gkn.guannengcc.top

[R32] 参数个数校验
来源：http://bmw.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sol.aizwys.cn

[R33] 捕获错误并提示行号
来源：http://ida.yangfankeji.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bbr.cqqwz.cn

[R34] 退出时清理
来源：http://vns.mhx1999.top

trap 'rm -f "$tmp"' EXIT
来源：http://phc.smart0.xyz

[R35] 后台执行并等待
来源：http://qqi.9152youxi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rel.jinyuanbaomall.cn

[R36] 并发执行多个任务
来源：http://ioo.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aaf.9152youxi.cn

[R37] 把输出赋给变量
来源：http://plz.zhijiandao.cn

files=$(ls -1)
来源：http://czi.cqqwz.cn

[R38] 管道串联
来源：http://cnj.andypj.xyz

cat a.txt | grep -i error | wc -l
来源：http://ybm.0kj1m.cn

[R39] 重定向标准输出与错误
来源：http://rgs.shanyushiyangtech.top

cmd > out.log 2>&1
来源：http://eia.dashuyun.cn

[R40] 追加写日志
来源：http://dbw.dashuyun.cn

echo "log" >> out.log
来源：http://vkd.birdmap.top

[R41] 丢弃输出
来源：http://sln.sxryk.cn

cmd >/dev/null 2>&1
来源：http://bgu.bjfxy.top

[R42] 输入重定向
来源：http://fam.tianlin.xyz

wc -l < a.txt
来源：http://eex.uphjek.com

[R43] 按名字查找文件
来源：http://upc.jinyuanbaomall.cn

find . -name "*.log" -type f
来源：http://qnq.hywenlv.cn

[R44] 按修改时间查找
来源：http://ykg.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://ljd.nanxinkj.top

[R45] 批量删除
来源：http://nes.ybcxt.top

find . -name "*.tmp" -delete
来源：http://cdv.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://pod.hywenlv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lpr.bjfxy.top

[R47] sed 单行替换
来源：http://var.gotoacloud.top

sed -i 's/foo/bar/g' a.txt
来源：http://hub.gotoacloud.top

[R48] awk 取指定列
来源：http://unm.jinqigufen.top

awk '{print $1, $3}' a.txt
来源：http://ybv.epnwcf.com

[R49] awk 带条件
来源：http://tei.fengsongda.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://orw.bjfxy.top

[R50] awk 求和
来源：http://mqv.nanxinkj.top

awk '{s += $2} END {print s}' a.txt
来源：http://twj.jyoumei.cn

[R51] 排序去重取前几
来源：http://yoa.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fnl.pycfn.com

[R52] 统计行数
来源：http://iiu.yongpay.top

wc -l a.txt
来源：http://zqm.yongpay.top

[R53] 查看文件头与实时尾
来源：http://pxe.havefunace.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zqq.hesvh.cn

[R54] 比较两个文件
来源：http://aee.sweek.top

diff a.txt b.txt
来源：http://dwq.hysaishi.cn

[R55] 压缩与解压
来源：http://cmx.hongshengwenyu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kyf.zhiwuduotai.top

[R56] 远程拷贝
来源：http://zmj.tian-w.cn

scp file user@host:/path/
来源：http://gtp.zhixingplan.top

[R57] 远程执行命令
来源：http://afq.sweek.top

ssh user@host 'uptime'
来源：http://qzo.tarul.cn

[R58] 下载文件
来源：http://kqo.0kj1m.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vio.ydzc1.top

[R59] 发 POST JSON
来源：http://qyj.xuanzx.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://aqd.hnxiangtu.top

[R60] 只看 HTTP 状态码
来源：http://twa.yanxiufei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://awa.ctjpmb.com

[R61] 磁盘占用
来源：http://zmw.zhixingplan.top

df -h;  du -sh *
来源：http://gef.yonumen.top

[R62] 找最占空间的文件
来源：http://gny.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://anj.zdbjq.cn

[R63] 内存与进程
来源：http://poj.zhaomingkeji.xyz

free -h;  ps aux | grep nginx
来源：http://rjh.c1oappe.top

[R64] 结束进程
来源：http://upp.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://str.yanxiufei.cn

[R65] 查看端口占用
来源：http://cjb.guannengcc.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rmj.316326.xyz

[R66] 定时任务
来源：http://buy.fzhhl.top

crontab -e;  crontab -l
来源：http://ilv.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://ymf.hammf.cn

openssl rand -hex 16
来源：http://fze.jinghuilouyu.cn

[R68] 计算文件校验值
来源：http://dbb.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://btp.guowangkeji.top

[R69] 生成随机密码
来源：http://frc.jqgufenzy.top

head -c 16 /dev/urandom | base64
来源：http://lae.meibo888.top

[R70] 时间戳与互转
来源：http://ulk.xziqi.cn

date +%s;  date -d @1700000000
来源：http://obq.hnxiangtu.top

[R71] 日期格式化
来源：http://oxi.jlsjyb.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dnn.tanke756.top

[R72] 等待端口就绪
来源：http://gcu.quarkkingdee.top

until nc -z localhost 3306; do sleep 1; done
来源：http://oxm.gogol.net.cn

[R73] 分割大日志
来源：http://weu.sufxvd.cn

split -l 1000 big.log part_
来源：http://ljs.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://sxl.zdqjudy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://inr.yonumen.top

[R75] 导出环境变量
来源：http://erb.epnwcf.com

export PATH="$HOME/bin:$PATH"
来源：http://gej.yj202588.top

[R76] 使用临时文件
来源：http://exg.tian-w.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qfn.sufxvd.cn

[R77] 读取用户输入
来源：http://deq.snrcjt.cn

read -rp "请输入: " ans
来源：http://djv.yj202588.top

[R78] 交互式菜单
来源：http://wcm.yanxiufei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bir.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://ugy.zhengqikj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vew.tanke756.top

[R80] 查看脚本执行耗时
来源：http://ztk.gaohongyu789.top

time ./run.sh
来源：http://etr.sufxvd.cn

================================================================================
来源：http://sje.bbcook.cn

S. C / C++ 专题
来源：http://zfd.shangyingyoupin.top

================================================================================
来源：http://emp.jinyuanbaomall.cn

[S01] C：Hello World
来源：http://jcj.hongshengwenyu.top

#include <stdio.h>
来源：http://kgu.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bsq.daria6918.cn

[S02] C：变量与格式化输出
来源：http://bkl.zhixingplan.top

int a = 10; printf("%d\n", a);
来源：http://rut.guannengcc.top

[S03] C：读入整数
来源：http://ayt.hcnkem.com

int x; scanf("%d", &x);
来源：http://rcl.hysaishi.cn

[S04] C：字符串复制
来源：http://pxx.tanke756.top

char dst[32]; strcpy(dst, "hi");
来源：http://rji.jyoumei.cn

[S05] C：字符串长度
来源：http://lxf.fzhhl.top

strlen(s)
来源：http://yvt.cqqwz.cn

[S06] C：字符串比较
来源：http://cmb.bjfxy.top

strcmp(a, b) == 0
来源：http://dzt.fehbvm.com

[S07] C：数组遍历求和
来源：http://ijt.vqdsnc.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ccq.gzhubu.top

[S08] C：动态内存分配与释放
来源：http://pxy.meibo888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xkk.jinyuanbaomall.cn

[S09] C：结构体定义与初始化
来源：http://hxo.yj20258888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uhv.birdmap.top

[S10] C：指针与解引用
来源：http://kpa.ywan-chungtsiang.top

int *p = &a;  *p = 5;
来源：http://lku.dianchejie.cn

[S11] C：逐行读文件
来源：http://hcm.tian-w.cn

FILE *f = fopen("a.txt", "r");
来源：http://wng.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wpf.xingfuxueyuan.xyz

fclose(f);
来源：http://wdk.shanyushiyangkeji.top

[S12] C：写文件
来源：http://bnv.jlsjyb.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jnc.sjlbkw.cn

[S13] C：宏定义
来源：http://ymp.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vny.yongpay.top

[S14] C：枚举
来源：http://hkb.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://fyn.iojbl.cn

[S15] C：类型转换
来源：http://yen.cdnleiting.top

(double) a / b
来源：http://yke.cdnleiting.top

[S16] C：位操作置位
来源：http://clu.aibaodan.cn

x |= (1 << 3);
来源：http://jyc.jinghuilouyu.cn

[S17] C：安全拼接字符串
来源：http://wyv.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://csr.316326.xyz

[S18] C：命令行参数
来源：http://som.aizwys.cn

int main(int argc, char **argv)
来源：http://upw.vqdsnc.cn

[S19] C：快速排序
来源：http://deh.shanyushiyangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://drr.yueranfly.top

[S20] C：二分查找
来源：http://zct.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cpi.0kj1m.cn

[S21] C：字符类别判断
来源：http://ojl.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ibx.tian-w.cn

[S22] C：字符串转数字
来源：http://rbl.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://vzg.jinyuanbaomall.cn

[S23] C：随机数
来源：http://yld.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xag.sufxvd.cn

[S24] C：获取本地时间
来源：http://czw.gotoacloud.top


<!-- 参考信息 -->