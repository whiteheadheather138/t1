代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lfe.ppjwa.cn

[Q54] 清空表
来源：http://loq.tianlin.xyz

TRUNCATE TABLE logs;
来源：http://rdc.jinghuilouyu.cn

[Q55] 排名（并列占位）
来源：http://klt.gaohongyu789.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ldv.sxryk.cn

[Q56] 密集排名（并列不占位）
来源：http://xld.yj20258888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yvi.jqgufenzy.top

[Q57] 行号
来源：http://oxk.iojbl.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mul.316326.xyz

[Q58] 累计求和
来源：http://rzf.fanxiaobao.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hwd.gaohongyu789.top

[Q59] 分组内累计
来源：http://djg.ehwqpu.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lvq.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://bqw.daria6918.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lcy.daria6918.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xrz.yj20258888.top

[Q61] 移动平均
来源：http://lpi.xylfe.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zjs.yongpay.top

[Q62] 分组占比
来源：http://jmv.xingfuxueyuan.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bxf.fanxiaobao.xyz

[Q63] 开启事务
来源：http://tay.sysykeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sbp.xingfuxueyuan.xyz

[Q64] 提交事务
来源：http://rxg.guannengcc.top

COMMIT;
来源：http://nkz.ydzc1.top

[Q65] 回滚事务
来源：http://vkb.gaohongyu789.top

ROLLBACK;
来源：http://hwx.nanxuanxn.top

[Q66] 行锁查询
来源：http://bxv.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kcq.c1oappe.top

[Q67] 设置隔离级别
来源：http://urd.haohaochexian.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ypi.sweek.top

[Q68] 保存点
来源：http://fiy.aizwys.cn

SAVEPOINT sp1;
来源：http://hai.yangfankeji.com

ROLLBACK TO sp1;
来源：http://iaw.shanyushiyangtech.top

[Q69] 查看执行计划
来源：http://oxu.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fdx.yvedp.cn

[Q70] 更新统计信息
来源：http://sdl.tian-w.cn

ANALYZE TABLE users;
来源：http://bui.hongshengwenyu.top

[Q71] 查看建表语句
来源：http://hco.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://utr.aibaodan.cn

[Q72] 查看索引
来源：http://gll.yongpay.top

SHOW INDEX FROM users;
来源：http://kev.haohaochexian.top

[Q73] 查看表状态
来源：http://ntw.daria6918.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mjd.zhiwuduotai.top

[Q74] 强制使用索引
来源：http://xpo.bjfxy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ace.yj20258888.top

[Q75] 日期格式化
来源：http://rjd.yvedp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://apg.tian-w.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zax.hammf.cn

[Q76] 按天统计
来源：http://uhc.ywan-chungtsiang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://avl.xinyue.icu

[Q77] 时间加减
来源：http://ybd.fktsv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ltv.cucudq.cn

[Q78] 当前时间
来源：http://ywu.yuxming.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jpv.ehwqpu.com

[Q79] 字符串拼接
来源：http://dmj.shuidangran.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iof.jinqigufen.top

[Q80] 字符串截取
来源：http://qfs.redwolf501.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://koe.aibaodan.cn

[Q81] 字符串替换
来源：http://ptl.xuanzx.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jkm.yanxiufei.cn

[Q82] 字符长度与字节长度
来源：http://qmr.pycfn.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://srn.svipenyu.cn

[Q83] 大小写转换
来源：http://qyb.yuxming.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ifo.yj20258.top

[Q84] 去除首尾空格
来源：http://yzu.nanxinkj.top

SELECT TRIM(name) FROM users;
来源：http://yfj.sweek.top

[Q85] 数值取整
来源：http://uxw.yfazqb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rfg.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://wkf.zhiwuduotai.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://khj.hammf.cn

[Q87] JSON 字段做条件
来源：http://miv.ctjpmb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nlj.ydzc1.top

[Q88] 行转列（条件聚合）
来源：http://peq.yanxiufei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cjl.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://htj.jqgufenzy.top

[Q89] 判断表是否存在
来源：http://eez.redwolf501.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zji.iojbl.cn

[Q90] 生成序号列
来源：http://lge.yj20258888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iwc.shuidangran.top

================================================================================
来源：http://upi.bbcook.cn

R. Bash 专题
来源：http://epb.sweek.top

================================================================================
来源：http://jzp.chenzaomai.com

[R01] shebang 与严格模式
来源：http://bgc.jianghu66.top

#!/usr/bin/env bash
来源：http://wpe.ppjwa.cn

set -euo pipefail
来源：http://bac.nwbrower.top

[R02] 变量赋值与使用
来源：http://tqs.sxryk.cn

name="Tom"; echo "$name"
来源：http://xvq.zhaomingkeji.xyz

[R03] 只读变量
来源：http://ryu.wangshuangyany.cn

readonly PI=3.14
来源：http://qwz.fengsongda.top

[R04] 位置参数
来源：http://kxi.xingfuxueyuan.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wpg.hcnkem.com

[R05] 参数默认值
来源：http://vnc.jinqigfzy.top

name="${1:-default}"
来源：http://eil.gogol.net.cn

[R06] 判断命令是否存在
来源：http://ksh.redwolf501.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vmb.vehdjk.com

[R07] if 判断文件
来源：http://dnt.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gmm.daria6918.cn

[R08] 数值比较
来源：http://qww.jyoumei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vog.zhoulong.xyz

[R09] 字符串比较
来源：http://xzu.havefunace.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fbt.aibaodan.cn

[R10] 正则匹配
来源：http://rrd.chenlongwang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lcq.tianlin.xyz

[R11] case 多分支
来源：http://rwd.havefunace.top

case "$1" in
来源：http://fkt.guannengcc.top

start) echo "启动" ;;
来源：http://pnk.zdbjq.cn

stop)  echo "停止" ;;
来源：http://inn.ivvv.top

*)     echo "未知命令" ;;
来源：http://ipb.yongpay.top

esac
来源：http://bix.yj20258888.top

[R12] for 遍历文件
来源：http://sig.xuanzx.com

for f in *.txt; do echo "$f"; done
来源：http://dgf.cashguo.top

[R13] for 计数循环
来源：http://npu.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://mmk.birdmap.top

[R14] C 风格 for
来源：http://ulj.guowangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://adz.ehwqpu.com

[R15] while 逐行读文件
来源：http://ujg.0kj1m.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qxv.cqqwz.cn

[R16] until 等待条件
来源：http://tsq.xuetiantiany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pgp.tarul.cn

[R17] 数组定义与取值
来源：http://kaw.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://ceo.mhx1999.top

[R18] 遍历数组
来源：http://xws.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rfq.hcnkem.com

[R19] 数组长度
来源：http://lwr.iojbl.cn

echo "${#arr[@]}"
来源：http://lhs.hfpthk.cn

[R20] 关联数组（字典）
来源：http://rvf.jiagoushi.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hib.mhx1999.top

[R21] 字符串长度
来源：http://dba.meibo888.top

echo "${#s}"
来源：http://lqz.zdqjudy.top

[R22] 截取子串
来源：http://uxi.feifeiyinyue.top

echo "${s:0:5}"
来源：http://opk.sufxvd.cn

[R23] 字符串替换
来源：http://kar.nanxuanxn.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pym.yj20258888.top

[R24] 大小写转换
来源：http://mpd.9152youxi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tur.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://cpy.jinghuilouyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ert.sweek.top

[R26] 命令替换
来源：http://vzg.c1oappe.top

now=$(date +%F); echo "$now"
来源：http://nsf.shangyingyoupin.top

[R27] 算术展开
来源：http://pci.bjfxy.top

echo $((1 + 2 * 3))
来源：http://sdp.feifeiyinyue.top

[R28] 浮点运算
来源：http://tpt.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://dps.feifeiyinyue.top

[R29] 定义函数
来源：http://bkj.yuanzhike.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xkn.yfazqb.com

[R30] 函数返回状态码
来源：http://xwt.fanxiaobao.xyz

f() { return 0; }; f || echo "失败了"
来源：http://stn.tian-w.cn

[R31] 局部变量
来源：http://hib.shuidangran.top

f() { local x=1; echo "$x"; }
来源：http://uop.wangdashe.top

[R32] 参数个数校验
来源：http://ryk.shanyushiyangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mrp.yuxming.cn

[R33] 捕获错误并提示行号
来源：http://ajh.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://juw.shangyingyoupin.top

[R34] 退出时清理
来源：http://zjq.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://eth.jinqigfzy.top

[R35] 后台执行并等待
来源：http://cgv.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mhj.jinqigufen.top

[R36] 并发执行多个任务
来源：http://qcl.hfpthk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://emd.redwolf501.top

[R37] 把输出赋给变量
来源：http://ouh.jianghu66.top

files=$(ls -1)
来源：http://rua.316326.xyz

[R38] 管道串联
来源：http://xnf.ywan-chungtsiang.top

cat a.txt | grep -i error | wc -l
来源：http://tra.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://wnx.zhengqikj.top

cmd > out.log 2>&1
来源：http://doc.52xcode.cn

[R40] 追加写日志
来源：http://pqb.daxiang520.top

echo "log" >> out.log
来源：http://vmq.yj20258888.top

[R41] 丢弃输出
来源：http://xzl.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://vmr.316326.xyz

[R42] 输入重定向
来源：http://pur.ctjpmb.com

wc -l < a.txt
来源：http://cqf.iojbl.cn

[R43] 按名字查找文件
来源：http://ifa.9152youxi.cn

find . -name "*.log" -type f
来源：http://sxl.nanxinkj.top

[R44] 按修改时间查找
来源：http://uxe.sjlbkw.cn

find . -mtime -7 -type f
来源：http://utn.quarkkingdee.top

[R45] 批量删除
来源：http://mki.ywan-chungtsiang.top

find . -name "*.tmp" -delete
来源：http://bcu.yongpay.top

[R46] 递归替换文件内容
来源：http://owf.ydzc1.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mfp.jqgufenzy.top

[R47] sed 单行替换
来源：http://xwc.sxryk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gdh.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://vst.guowangkeji.top

awk '{print $1, $3}' a.txt
来源：http://mds.feifeiyinyue.top

[R49] awk 带条件
来源：http://qry.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tsx.zhiwuduotai.top

[R50] awk 求和
来源：http://ycf.sjlbkw.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jhw.ydjk.org.cn

[R51] 排序去重取前几
来源：http://gzp.jinyuanbaomall.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dny.xuanzx.com

[R52] 统计行数
来源：http://cvu.zdqjudy.top

wc -l a.txt
来源：http://bbo.yvedp.cn

[R53] 查看文件头与实时尾
来源：http://pop.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rxi.epnwcf.com

[R54] 比较两个文件
来源：http://yqy.jinyuanbaomall.cn

diff a.txt b.txt
来源：http://gio.daxiang520.top

[R55] 压缩与解压
来源：http://zvq.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://grj.sysykeji.top

[R56] 远程拷贝
来源：http://ory.aibaodan.cn

scp file user@host:/path/
来源：http://fky.fzhhl.top

[R57] 远程执行命令
来源：http://vit.gzhubu.top

ssh user@host 'uptime'
来源：http://tkd.wangdashe.top

[R58] 下载文件
来源：http://gmo.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xip.jinyuanbaomall.cn

[R59] 发 POST JSON
来源：http://jee.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mvq.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://mbp.xinyue.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iip.gotoacloud.top

[R61] 磁盘占用
来源：http://eak.yonumen.top

df -h;  du -sh *
来源：http://psr.zhixingplan.top

[R62] 找最占空间的文件
来源：http://upi.jianghu66.top

du -ah . | sort -rh | head -10
来源：http://qrk.jlsjyb.cn

[R63] 内存与进程
来源：http://aeh.wangdashe.top

free -h;  ps aux | grep nginx
来源：http://ljv.gzhubu.top

[R64] 结束进程
来源：http://naw.xuanzx.com

kill -9 $(pgrep -f app.py)
来源：http://duo.hywenlv.cn

[R65] 查看端口占用
来源：http://lkk.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uft.zhijiandao.cn

[R66] 定时任务
来源：http://rjy.tian-w.cn

crontab -e;  crontab -l
来源：http://ifz.bjfxy.top

[R67] 生成随机十六进制串
来源：http://wzq.hcnkem.com

openssl rand -hex 16
来源：http://mog.kuanghao11.cn

[R68] 计算文件校验值
来源：http://whv.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://nuq.epnwcf.com

[R69] 生成随机密码
来源：http://zer.cucudq.cn

head -c 16 /dev/urandom | base64
来源：http://rpf.fehbvm.com

[R70] 时间戳与互转
来源：http://bsp.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://fsa.feifeiyinyue.top

[R71] 日期格式化
来源：http://xpm.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://lep.xziqi.cn

[R72] 等待端口就绪
来源：http://cio.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bmz.gotoacloud.top

[R73] 分割大日志
来源：http://qlk.andypj.xyz

split -l 1000 big.log part_
来源：http://swe.shuidangran.top

[R74] 批量重命名
来源：http://nqr.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tsg.yj202588.top

[R75] 导出环境变量
来源：http://tii.cashguo.top

export PATH="$HOME/bin:$PATH"
来源：http://fiz.jinqigfzy.top

[R76] 使用临时文件
来源：http://tpr.sufxvd.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rny.shzxlz.cn

[R77] 读取用户输入
来源：http://fub.ctjpmb.com

read -rp "请输入: " ans
来源：http://hid.gogol.net.cn

[R78] 交互式菜单
来源：http://bdj.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dxi.jqgfzy.top

[R79] 解析命令行选项
来源：http://hnb.jinghuilouyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nun.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://pri.dashuyun.cn

time ./run.sh
来源：http://rig.ppjwa.cn

================================================================================
来源：http://btf.guowangkeji.top

S. C / C++ 专题
来源：http://epe.yj20258.top

================================================================================
来源：http://fbb.ydjk.org.cn

[S01] C：Hello World
来源：http://jia.iojbl.cn

#include <stdio.h>
来源：http://kpl.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vnp.bbcook.cn

[S02] C：变量与格式化输出
来源：http://muw.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://dqs.birdmap.top

[S03] C：读入整数
来源：http://jkn.gogol.net.cn

int x; scanf("%d", &x);
来源：http://byu.ydzc1.top

[S04] C：字符串复制
来源：http://rib.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://qdv.hammf.cn

[S05] C：字符串长度
来源：http://mox.meibo888.top

strlen(s)
来源：http://ira.guowangkeji.top

[S06] C：字符串比较
来源：http://egg.ppjwa.cn

strcmp(a, b) == 0
来源：http://xug.gogol.net.cn

[S07] C：数组遍历求和
来源：http://uyf.havefunace.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jav.fengsongda.top

[S08] C：动态内存分配与释放
来源：http://abo.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wsv.52xcode.cn

[S09] C：结构体定义与初始化
来源：http://iph.316326.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://upy.ivvv.top

[S10] C：指针与解引用
来源：http://ail.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://wgq.tian-w.cn

[S11] C：逐行读文件
来源：http://rmi.yuanzhike.top

FILE *f = fopen("a.txt", "r");
来源：http://ner.pycfn.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://bji.jinqigfzy.top

fclose(f);
来源：http://vjz.haohaochexian.top

[S12] C：写文件
来源：http://ssr.snrcjt.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ntu.jyoumei.cn

[S13] C：宏定义
来源：http://dpi.smart0.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://osj.gzhubu.top

[S14] C：枚举
来源：http://wgk.jqgfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://rph.chenzaomai.com

[S15] C：类型转换
来源：http://nht.hnqzz.top

(double) a / b
来源：http://iiv.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://kcc.jinghuilouyu.cn

x |= (1 << 3);
来源：http://jvf.yuanzhike.top

[S17] C：安全拼接字符串
来源：http://nyw.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vqu.hongshengwenyu.top

[S18] C：命令行参数
来源：http://ifn.fktsv.cn

int main(int argc, char **argv)
来源：http://pyw.yangfankeji.com

[S19] C：快速排序
来源：http://yzq.hfpthk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xbk.kuanghao11.cn

[S20] C：二分查找
来源：http://hsp.aizwys.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fow.ydzc1.top

[S21] C：字符类别判断
来源：http://zxi.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qwx.cucudq.cn

[S22] C：字符串转数字
来源：http://yhn.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://cjd.shuidangran.top

[S23] C：随机数
来源：http://ebd.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ujq.ybcxt.top

[S24] C：获取本地时间
来源：http://gyz.jianghu66.top


<!-- 参考信息 -->