代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xlu.ydjk.org.cn

[Q50] 批量更新
来源：http://rpn.hfpthk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fpg.9152youxi.cn

[Q51] 用子查询更新
来源：http://sna.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qay.pengpengdd.cyou

[Q52] 删除指定行
来源：http://pxh.52xcode.cn

DELETE FROM users WHERE id = 10;
来源：http://wko.birdmap.top

[Q53] 按条件删除
来源：http://ogt.sysykeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ybx.vqdsnc.cn

[Q54] 清空表
来源：http://bpa.c1oappe.top

TRUNCATE TABLE logs;
来源：http://zht.andypj.xyz

[Q55] 排名（并列占位）
来源：http://bzr.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gde.zhoulong.xyz

[Q56] 密集排名（并列不占位）
来源：http://sjd.dianchejie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gzq.mhx1999.top

[Q57] 行号
来源：http://ohk.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://idw.yongpay.top

[Q58] 累计求和
来源：http://lkf.sweek.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gfm.52xcode.cn

[Q59] 分组内累计
来源：http://pyr.hnxiangtu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xak.9152youxi.cn

[Q60] 取上一行 / 下一行
来源：http://umz.wangshuangyany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jvz.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gqv.gaohongyu789.top

[Q61] 移动平均
来源：http://hyv.jqgfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rms.mhx1999.top

[Q62] 分组占比
来源：http://nlq.hnqzz.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vrc.tian-w.cn

[Q63] 开启事务
来源：http://olj.zdbjq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vlj.jlsjyb.cn

[Q64] 提交事务
来源：http://rwa.redwolf501.top

COMMIT;
来源：http://ftz.hfpthk.cn

[Q65] 回滚事务
来源：http://flq.ydjk.org.cn

ROLLBACK;
来源：http://pcd.pycfn.com

[Q66] 行锁查询
来源：http://nxc.ehwqpu.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jph.mhx1999.top

[Q67] 设置隔离级别
来源：http://pwe.wangshuangyany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fkl.fanxiaobao.xyz

[Q68] 保存点
来源：http://ult.fanxiaobao.xyz

SAVEPOINT sp1;
来源：http://rzm.jinghuilouyu.cn

ROLLBACK TO sp1;
来源：http://tdz.ydjk.org.cn

[Q69] 查看执行计划
来源：http://gxa.316326.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vjm.ydjk.org.cn

[Q70] 更新统计信息
来源：http://ssu.shzxlz.cn

ANALYZE TABLE users;
来源：http://qhi.zhengqikj.top

[Q71] 查看建表语句
来源：http://kom.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://euj.yangfankeji.com

[Q72] 查看索引
来源：http://upa.zhongyouzk.top

SHOW INDEX FROM users;
来源：http://zgx.yangfankeji.com

[Q73] 查看表状态
来源：http://iua.gotoacloud.top

SHOW TABLE STATUS LIKE 'users';
来源：http://cip.52xcode.cn

[Q74] 强制使用索引
来源：http://yoy.jlsjyb.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xyb.nanxuanxn.top

[Q75] 日期格式化
来源：http://oyw.ywan-chungtsiang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lah.jqgfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qgx.yangfankeji.com

[Q76] 按天统计
来源：http://thx.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bnv.hywenlv.cn

[Q77] 时间加减
来源：http://jpa.meibo888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bhk.yongpay.top

[Q78] 当前时间
来源：http://jow.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yvr.zdqjudy.top

[Q79] 字符串拼接
来源：http://kvr.nwbrower.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lsx.52xcode.cn

[Q80] 字符串截取
来源：http://hwh.yanxiufei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://huc.shangyingyoupin.top

[Q81] 字符串替换
来源：http://isr.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qws.jqgufenzy.top

[Q82] 字符长度与字节长度
来源：http://fev.cdnleiting.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://psb.daxiang520.top

[Q83] 大小写转换
来源：http://qyi.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mqa.sufxvd.cn

[Q84] 去除首尾空格
来源：http://sso.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://trr.xylfe.cn

[Q85] 数值取整
来源：http://jtr.hongshengwenyu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kyz.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://wqh.fengsongda.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dth.epnwcf.com

[Q87] JSON 字段做条件
来源：http://gba.yj20258.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ouo.zycfv.cn

[Q88] 行转列（条件聚合）
来源：http://nbr.fzhhl.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hqi.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rxb.vehdjk.com

[Q89] 判断表是否存在
来源：http://sie.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sax.pengpengdd.cyou

[Q90] 生成序号列
来源：http://cpo.birdmap.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bed.epnwcf.com

================================================================================
来源：http://gio.hfpthk.cn

R. Bash 专题
来源：http://iur.yfazqb.com

================================================================================
来源：http://tdc.yuxming.cn

[R01] shebang 与严格模式
来源：http://ewn.zhongyouzk.top

#!/usr/bin/env bash
来源：http://wfz.yuxming.cn

set -euo pipefail
来源：http://qcn.jianghu66.top

[R02] 变量赋值与使用
来源：http://etd.dianchejie.cn

name="Tom"; echo "$name"
来源：http://gob.pengpengdd.cyou

[R03] 只读变量
来源：http://btj.jyoumei.cn

readonly PI=3.14
来源：http://oir.sweek.top

[R04] 位置参数
来源：http://uxe.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ael.zycfv.cn

[R05] 参数默认值
来源：http://vwp.guowangkeji.top

name="${1:-default}"
来源：http://qyw.gogol.net.cn

[R06] 判断命令是否存在
来源：http://twd.kuanghao11.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vuf.yj20258888.top

[R07] if 判断文件
来源：http://rbw.quarkkingdee.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://psr.guannengcc.top

[R08] 数值比较
来源：http://kwq.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wkn.chenjidiqi.icu

[R09] 字符串比较
来源：http://mwj.zhixingplan.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ssz.yonumen.top

[R10] 正则匹配
来源：http://wed.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://utx.gzhubu.top

[R11] case 多分支
来源：http://qpt.zycfv.cn

case "$1" in
来源：http://cyr.tian-w.cn

start) echo "启动" ;;
来源：http://vgu.pengpengdd.cyou

stop)  echo "停止" ;;
来源：http://tns.jyoumei.cn

*)     echo "未知命令" ;;
来源：http://yyq.316326.xyz

esac
来源：http://euz.cucudq.cn

[R12] for 遍历文件
来源：http://efw.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://iua.shanyushiyangkeji.top

[R13] for 计数循环
来源：http://qju.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://bga.chenlongwang.top

[R14] C 风格 for
来源：http://aql.redwolf501.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://viu.jinqigufen.top

[R15] while 逐行读文件
来源：http://amz.cashguo.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://thu.hongshengwenyu.top

[R16] until 等待条件
来源：http://usq.nanxinkj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cpd.fengsongda.top

[R17] 数组定义与取值
来源：http://eoi.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oiw.jianghu66.top

[R18] 遍历数组
来源：http://ymv.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eyc.quarkkingdee.top

[R19] 数组长度
来源：http://jin.vehdjk.com

echo "${#arr[@]}"
来源：http://vkl.chenjidiqi.icu

[R20] 关联数组（字典）
来源：http://jzc.birdmap.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ycd.hcnkem.com

[R21] 字符串长度
来源：http://maf.shangyingyoupin.top

echo "${#s}"
来源：http://nrf.zhixingplan.top

[R22] 截取子串
来源：http://nwr.zhaomingkeji.xyz

echo "${s:0:5}"
来源：http://mjw.sjlbkw.cn

[R23] 字符串替换
来源：http://brt.yonumen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qop.haohaochexian.top

[R24] 大小写转换
来源：http://kke.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://eql.sweek.top

[R25] 去后缀 / 去前缀
来源：http://eua.sxryk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://csa.wangdashe.top

[R26] 命令替换
来源：http://rxn.shanyushiyangtech.top

now=$(date +%F); echo "$now"
来源：http://qeo.nwbrower.top

[R27] 算术展开
来源：http://jyc.yj202588.top

echo $((1 + 2 * 3))
来源：http://ato.dianchejie.cn

[R28] 浮点运算
来源：http://wfu.wangshuangyany.cn

echo "scale=2; 10/3" | bc
来源：http://jxn.yfazqb.com

[R29] 定义函数
来源：http://tnm.jlsjyb.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rdw.zhoulong.xyz

[R30] 函数返回状态码
来源：http://iqz.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://buo.dashuyun.cn

[R31] 局部变量
来源：http://uvq.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://ykk.jiagoushi.top

[R32] 参数个数校验
来源：http://fdw.jinqigfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zhz.wangdashe.top

[R33] 捕获错误并提示行号
来源：http://usb.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iou.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://fxn.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://tqs.xziqi.cn

[R35] 后台执行并等待
来源：http://ibx.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://cun.zhongyouzk.top

[R36] 并发执行多个任务
来源：http://xue.xingfuxueyuan.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wjd.zycfv.cn

[R37] 把输出赋给变量
来源：http://zbg.jinyuanbaomall.cn

files=$(ls -1)
来源：http://jqh.hcnkem.com

[R38] 管道串联
来源：http://zel.jinghuilouyu.cn

cat a.txt | grep -i error | wc -l
来源：http://zbq.jyoumei.cn

[R39] 重定向标准输出与错误
来源：http://wfg.snrcjt.cn

cmd > out.log 2>&1
来源：http://tbf.fehbvm.com

[R40] 追加写日志
来源：http://xdu.fktsv.cn

echo "log" >> out.log
来源：http://qra.sweek.top

[R41] 丢弃输出
来源：http://cjp.sxryk.cn

cmd >/dev/null 2>&1
来源：http://fft.epnwcf.com

[R42] 输入重定向
来源：http://joj.jinqigfzy.top

wc -l < a.txt
来源：http://dzj.chenzaomai.com

[R43] 按名字查找文件
来源：http://qzp.ppjwa.cn

find . -name "*.log" -type f
来源：http://izr.kuanghao11.cn

[R44] 按修改时间查找
来源：http://acm.0kj1m.cn

find . -mtime -7 -type f
来源：http://xks.iojbl.cn

[R45] 批量删除
来源：http://uqb.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://hal.birdmap.top

[R46] 递归替换文件内容
来源：http://hyk.jqgufenzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zud.guowangkeji.top

[R47] sed 单行替换
来源：http://ufy.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://cvr.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://jqo.quarkkingdee.top

awk '{print $1, $3}' a.txt
来源：http://wwj.ywan-chungtsiang.top

[R49] awk 带条件
来源：http://fmz.fehbvm.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bpr.aibaodan.cn

[R50] awk 求和
来源：http://rpe.hnqzz.top

awk '{s += $2} END {print s}' a.txt
来源：http://gqp.jianghu66.top

[R51] 排序去重取前几
来源：http://kgl.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ugd.iojbl.cn

[R52] 统计行数
来源：http://ysc.kuanghao11.cn

wc -l a.txt
来源：http://xlo.ydjk.org.cn

[R53] 查看文件头与实时尾
来源：http://qqc.zhongyouzk.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ajz.52xcode.cn

[R54] 比较两个文件
来源：http://put.cheryme.top

diff a.txt b.txt
来源：http://hwl.hfpthk.cn

[R55] 压缩与解压
来源：http://laq.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gld.hywenlv.cn

[R56] 远程拷贝
来源：http://vbc.uphjek.com

scp file user@host:/path/
来源：http://gbm.snrcjt.cn

[R57] 远程执行命令
来源：http://ndq.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://ucb.daria6918.cn

[R58] 下载文件
来源：http://okd.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pwn.tarul.cn

[R59] 发 POST JSON
来源：http://xrw.hcnkem.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ofj.guowangkeji.top

[R60] 只看 HTTP 状态码
来源：http://eym.wangshuangyany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zfp.ydzc1.top

[R61] 磁盘占用
来源：http://oxt.redwolf501.top

df -h;  du -sh *
来源：http://woo.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://ecn.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://orf.bjfxy.top

[R63] 内存与进程
来源：http://frf.cucudq.cn

free -h;  ps aux | grep nginx
来源：http://wtw.gaohongyu789.top

[R64] 结束进程
来源：http://brj.316326.xyz

kill -9 $(pgrep -f app.py)
来源：http://xnh.zhiwuduotai.top

[R65] 查看端口占用
来源：http://kfp.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wkg.shuidangran.top

[R66] 定时任务
来源：http://pxg.hammf.cn

crontab -e;  crontab -l
来源：http://dyd.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://ohj.ydjk.org.cn

openssl rand -hex 16
来源：http://laq.snrcjt.cn

[R68] 计算文件校验值
来源：http://mjl.zhiwuduotai.top

sha256sum a.txt;  md5sum a.txt
来源：http://iry.jqgfzy.top

[R69] 生成随机密码
来源：http://mix.birdmap.top

head -c 16 /dev/urandom | base64
来源：http://zpr.gzhubu.top

[R70] 时间戳与互转
来源：http://rxc.gzhubu.top

date +%s;  date -d @1700000000
来源：http://jwq.bbcook.cn

[R71] 日期格式化
来源：http://wdb.nanxinkj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rkt.zdqjudy.top

[R72] 等待端口就绪
来源：http://mkr.hongshengwenyu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hhm.hnxiangtu.top

[R73] 分割大日志
来源：http://bwp.cqqwz.cn

split -l 1000 big.log part_
来源：http://isb.hcnkem.com

[R74] 批量重命名
来源：http://hhl.yvedp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nvk.haohaochexian.top

[R75] 导出环境变量
来源：http://jvw.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://ijp.sxryk.cn

[R76] 使用临时文件
来源：http://ilk.andypj.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ekg.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://vzp.ydjk.org.cn

read -rp "请输入: " ans
来源：http://oom.yuanzhike.top

[R78] 交互式菜单
来源：http://dal.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://egf.tianlin.xyz

[R79] 解析命令行选项
来源：http://cjp.fzhhl.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rmo.chenlongwang.top

[R80] 查看脚本执行耗时
来源：http://iie.ppjwa.cn

time ./run.sh
来源：http://rkg.fehbvm.com

================================================================================
来源：http://pcg.guowangkeji.top

S. C / C++ 专题
来源：http://czs.hcnkem.com

================================================================================
来源：http://zsw.ppjwa.cn

[S01] C：Hello World
来源：http://osa.jianghu66.top

#include <stdio.h>
来源：http://hjb.aizwys.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kjb.daria6918.cn

[S02] C：变量与格式化输出
来源：http://gxq.mhx1999.top

int a = 10; printf("%d\n", a);
来源：http://prx.sjlbkw.cn

[S03] C：读入整数
来源：http://fuo.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://keq.redwolf501.top

[S04] C：字符串复制
来源：http://pcw.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wlb.sweek.top

[S05] C：字符串长度
来源：http://tsl.ehwqpu.com

strlen(s)
来源：http://gta.yj202588.top

[S06] C：字符串比较
来源：http://kxw.gaohongyu789.top

strcmp(a, b) == 0
来源：http://cnf.yangfankeji.com

[S07] C：数组遍历求和
来源：http://kkj.zhongyouzk.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pdn.hammf.cn

[S08] C：动态内存分配与释放
来源：http://sli.epnwcf.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rft.fzhhl.top

[S09] C：结构体定义与初始化
来源：http://plf.zhaomingkeji.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zuz.guannengcc.top

[S10] C：指针与解引用
来源：http://kbg.cheryme.top

int *p = &a;  *p = 5;
来源：http://sjw.jqgufenzy.top

[S11] C：逐行读文件
来源：http://zrr.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://dcl.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://yoe.pycfn.com

fclose(f);
来源：http://qtb.yonumen.top

[S12] C：写文件
来源：http://hkx.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xlp.jqgfzy.top

[S13] C：宏定义
来源：http://jvb.chenlongwang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://trp.xinyue.icu

[S14] C：枚举
来源：http://ord.meibo888.top

enum Color { RED, GREEN, BLUE };
来源：http://ujc.hywenlv.cn

[S15] C：类型转换
来源：http://ryr.sweek.top

(double) a / b
来源：http://ulq.hcnkem.com

[S16] C：位操作置位
来源：http://ptp.52xcode.cn

x |= (1 << 3);
来源：http://ude.zhoulong.xyz

[S17] C：安全拼接字符串
来源：http://jkh.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lmv.iojbl.cn

[S18] C：命令行参数
来源：http://nfv.vqdsnc.cn

int main(int argc, char **argv)
来源：http://pom.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://avh.jyoumei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bzs.cashguo.top

[S20] C：二分查找
来源：http://drj.ehwqpu.com


<!-- 参考信息 -->