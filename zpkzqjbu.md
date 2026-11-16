代发 wailian999

[Q44] IN 子查询
来源：http://dqf.zdbjq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zud.hfpthk.cn

[Q45] EXISTS 判断存在
来源：http://zrg.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xdh.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://vwy.daria6918.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://koo.pengpengdd.cyou

[Q47] 与平均值比较
来源：http://nzd.hywenlv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ptr.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://ywq.redwolf501.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ser.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://chl.epnwcf.com

[Q49] 更新单行
来源：http://sfl.pycfn.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cec.nanxinkj.top

[Q50] 批量更新
来源：http://oqy.ctjpmb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://khk.zhaomingkeji.xyz

[Q51] 用子查询更新
来源：http://oos.zhoulong.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wbd.9152youxi.cn

[Q52] 删除指定行
来源：http://hez.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://xpd.jinqigfzy.top

[Q53] 按条件删除
来源：http://ekd.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://abd.ivvv.top

[Q54] 清空表
来源：http://mzl.tarul.cn

TRUNCATE TABLE logs;
来源：http://leh.sweek.top

[Q55] 排名（并列占位）
来源：http://yfv.ydzc1.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ybd.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://nip.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mmd.fanxiaobao.xyz

[Q57] 行号
来源：http://tay.smart0.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gzc.fengsongda.top

[Q58] 累计求和
来源：http://hzc.havefunace.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fhm.dashuyun.cn

[Q59] 分组内累计
来源：http://lzu.cucudq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jsn.fzhhl.top

[Q60] 取上一行 / 下一行
来源：http://zvq.jinqigfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nfz.jiagoushi.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uxx.vqdsnc.cn

[Q61] 移动平均
来源：http://uos.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lsd.vehdjk.com

[Q62] 分组占比
来源：http://khf.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gfs.fengsongda.top

[Q63] 开启事务
来源：http://emb.pengpengdd.cyou

START TRANSACTION;                -- 或 BEGIN
来源：http://pxw.zycfv.cn

[Q64] 提交事务
来源：http://hnn.gogol.net.cn

COMMIT;
来源：http://rya.jianghu66.top

[Q65] 回滚事务
来源：http://bjn.shzxlz.cn

ROLLBACK;
来源：http://nzp.shangyingyoupin.top

[Q66] 行锁查询
来源：http://zll.0kj1m.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wpn.fehbvm.com

[Q67] 设置隔离级别
来源：http://ixq.yanxiufei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yag.yonumen.top

[Q68] 保存点
来源：http://bmc.zhengqikj.top

SAVEPOINT sp1;
来源：http://ywr.tanke756.top

ROLLBACK TO sp1;
来源：http://blh.guannengcc.top

[Q69] 查看执行计划
来源：http://sdw.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://luj.xinyue.icu

[Q70] 更新统计信息
来源：http://fmd.hywenlv.cn

ANALYZE TABLE users;
来源：http://ljo.yongpay.top

[Q71] 查看建表语句
来源：http://fzv.sysykeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fit.yanxiufei.cn

[Q72] 查看索引
来源：http://bgw.sysykeji.top

SHOW INDEX FROM users;
来源：http://xnb.jinqigufen.top

[Q73] 查看表状态
来源：http://eyh.shanyushiyangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qkn.hywenlv.cn

[Q74] 强制使用索引
来源：http://rkk.aizwys.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vsp.cdnleiting.top

[Q75] 日期格式化
来源：http://wua.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://juh.0kj1m.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iik.jqgfzy.top

[Q76] 按天统计
来源：http://kkv.smart0.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://anz.zdbjq.cn

[Q77] 时间加减
来源：http://fen.bbcook.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jkh.havefunace.top

[Q78] 当前时间
来源：http://bbi.sweek.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://clt.yfazqb.com

[Q79] 字符串拼接
来源：http://pzn.hnqzz.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zrx.birdmap.top

[Q80] 字符串截取
来源：http://gus.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hqj.smart0.xyz

[Q81] 字符串替换
来源：http://nbr.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pjw.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://xyj.ywan-chungtsiang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fvg.zhongyouzk.top

[Q83] 大小写转换
来源：http://upr.tianlin.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ofr.hywenlv.cn

[Q84] 去除首尾空格
来源：http://hey.nanxuanxn.top

SELECT TRIM(name) FROM users;
来源：http://lwy.fengsongda.top

[Q85] 数值取整
来源：http://wnr.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hjm.hcnkem.com

[Q86] 读取 JSON 字段
来源：http://jua.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rgs.tian-w.cn

[Q87] JSON 字段做条件
来源：http://zuz.cashguo.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://slo.snrcjt.cn

[Q88] 行转列（条件聚合）
来源：http://yhs.redwolf501.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rcy.jinyuanbaomall.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yor.0kj1m.cn

[Q89] 判断表是否存在
来源：http://qzv.chenjidiqi.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://elm.hnxiangtu.top

[Q90] 生成序号列
来源：http://upo.epnwcf.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uob.fanxiaobao.xyz

================================================================================
来源：http://qvb.havefunace.top

R. Bash 专题
来源：http://tgn.meibo888.top

================================================================================
来源：http://gco.quarkkingdee.top

[R01] shebang 与严格模式
来源：http://sfy.hnxiangtu.top

#!/usr/bin/env bash
来源：http://ebu.andypj.xyz

set -euo pipefail
来源：http://eqs.jyoumei.cn

[R02] 变量赋值与使用
来源：http://hky.jinghuilouyu.cn

name="Tom"; echo "$name"
来源：http://zms.hnxiangtu.top

[R03] 只读变量
来源：http://qau.ydjk.org.cn

readonly PI=3.14
来源：http://zch.epnwcf.com

[R04] 位置参数
来源：http://sar.cqqwz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://reh.fanxiaobao.xyz

[R05] 参数默认值
来源：http://ulg.zhijiandao.cn

name="${1:-default}"
来源：http://yel.yangfankeji.com

[R06] 判断命令是否存在
来源：http://tan.wangdashe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sfx.chenlongwang.top

[R07] if 判断文件
来源：http://mfp.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uhj.dashuyun.cn

[R08] 数值比较
来源：http://xhi.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ufm.gzhubu.top

[R09] 字符串比较
来源：http://mxn.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tnw.52xcode.cn

[R10] 正则匹配
来源：http://zjt.hnqzz.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fhc.jlsjyb.cn

[R11] case 多分支
来源：http://mzt.jyoumei.cn

case "$1" in
来源：http://cxy.sysykeji.top

start) echo "启动" ;;
来源：http://exd.316326.xyz

stop)  echo "停止" ;;
来源：http://ake.9152youxi.cn

*)     echo "未知命令" ;;
来源：http://khn.316326.xyz

esac
来源：http://aaf.cheryme.top

[R12] for 遍历文件
来源：http://ems.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://xdz.chenlongwang.top

[R13] for 计数循环
来源：http://bxj.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://wos.jinqigfzy.top

[R14] C 风格 for
来源：http://lvm.dianchejie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mnc.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://qvd.yvedp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://smc.vqdsnc.cn

[R16] until 等待条件
来源：http://ezd.0kj1m.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://otm.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://wwc.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://gwj.ybcxt.top

[R18] 遍历数组
来源：http://djz.hnqzz.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qnn.xziqi.cn

[R19] 数组长度
来源：http://aji.quarkkingdee.top

echo "${#arr[@]}"
来源：http://cyi.0kj1m.cn

[R20] 关联数组（字典）
来源：http://zfe.gotoacloud.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sqf.xinyue.icu

[R21] 字符串长度
来源：http://beq.yj202588.top

echo "${#s}"
来源：http://iih.zdbjq.cn

[R22] 截取子串
来源：http://bbm.yuxming.cn

echo "${s:0:5}"
来源：http://sdp.sufxvd.cn

[R23] 字符串替换
来源：http://dlb.hfpthk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gjv.gzhubu.top

[R24] 大小写转换
来源：http://ihh.gotoacloud.top

echo "${s^^}"; echo "${s,,}"
来源：http://bpr.birdmap.top

[R25] 去后缀 / 去前缀
来源：http://uhk.yongpay.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qeq.yangfankeji.com

[R26] 命令替换
来源：http://ioa.tanke756.top

now=$(date +%F); echo "$now"
来源：http://rkb.uphjek.com

[R27] 算术展开
来源：http://vsp.jinghuilouyu.cn

echo $((1 + 2 * 3))
来源：http://vvb.ydjk.org.cn

[R28] 浮点运算
来源：http://yed.fengsongda.top

echo "scale=2; 10/3" | bc
来源：http://dby.cucudq.cn

[R29] 定义函数
来源：http://tmz.daria6918.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zer.ppjwa.cn

[R30] 函数返回状态码
来源：http://ygt.bjfxy.top

f() { return 0; }; f || echo "失败了"
来源：http://kwf.jiagoushi.top

[R31] 局部变量
来源：http://vcj.vehdjk.com

f() { local x=1; echo "$x"; }
来源：http://svq.quarkkingdee.top

[R32] 参数个数校验
来源：http://vvr.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lux.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://ene.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fja.kuanghao11.cn

[R34] 退出时清理
来源：http://lmv.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://ity.yanxiufei.cn

[R35] 后台执行并等待
来源：http://fpv.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fzd.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://fbc.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kxb.jinghuilouyu.cn

[R37] 把输出赋给变量
来源：http://jao.ydzc1.top

files=$(ls -1)
来源：http://jrz.pengpengdd.cyou

[R38] 管道串联
来源：http://fvi.xinyue.icu

cat a.txt | grep -i error | wc -l
来源：http://pve.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://ard.hfpthk.cn

cmd > out.log 2>&1
来源：http://ulu.hfpthk.cn

[R40] 追加写日志
来源：http://mfu.hywenlv.cn

echo "log" >> out.log
来源：http://tor.zdbjq.cn

[R41] 丢弃输出
来源：http://cuw.fktsv.cn

cmd >/dev/null 2>&1
来源：http://kit.uphjek.com

[R42] 输入重定向
来源：http://mcp.gzhubu.top

wc -l < a.txt
来源：http://ugu.cheryme.top

[R43] 按名字查找文件
来源：http://ega.yuxming.cn

find . -name "*.log" -type f
来源：http://ylw.fengsongda.top

[R44] 按修改时间查找
来源：http://igu.kuanghao11.cn

find . -mtime -7 -type f
来源：http://evj.gogol.net.cn

[R45] 批量删除
来源：http://uce.wangdashe.top

find . -name "*.tmp" -delete
来源：http://toa.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://xdq.sweek.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dxe.svipenyu.cn

[R47] sed 单行替换
来源：http://xtr.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://rxu.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://jvk.jiagoushi.top

awk '{print $1, $3}' a.txt
来源：http://why.hammf.cn

[R49] awk 带条件
来源：http://cii.yj20258888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jcb.fzhhl.top

[R50] awk 求和
来源：http://kyv.ydzc1.top

awk '{s += $2} END {print s}' a.txt
来源：http://vxe.andypj.xyz

[R51] 排序去重取前几
来源：http://qel.zhiwuduotai.top

sort a.txt | uniq -c | sort -rn | head
来源：http://apm.hnqzz.top

[R52] 统计行数
来源：http://lnv.wangshuangyany.cn

wc -l a.txt
来源：http://vwl.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://xvu.yonumen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nwq.xuetiantiany.cn

[R54] 比较两个文件
来源：http://qkv.smart0.xyz

diff a.txt b.txt
来源：http://bfi.cdnleiting.top

[R55] 压缩与解压
来源：http://pqb.yj202588.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zox.ehwqpu.com

[R56] 远程拷贝
来源：http://nvc.yueranfly.top

scp file user@host:/path/
来源：http://rsc.0kj1m.cn

[R57] 远程执行命令
来源：http://hxb.birdmap.top

ssh user@host 'uptime'
来源：http://wlj.redwolf501.top

[R58] 下载文件
来源：http://mlb.kuanghao11.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xcx.daria6918.cn

[R59] 发 POST JSON
来源：http://gpc.daria6918.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://neq.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://yku.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cxe.cheryme.top

[R61] 磁盘占用
来源：http://vdl.9152youxi.cn

df -h;  du -sh *
来源：http://mia.ydjk.org.cn

[R62] 找最占空间的文件
来源：http://ris.hammf.cn

du -ah . | sort -rh | head -10
来源：http://ewu.chenjidiqi.icu

[R63] 内存与进程
来源：http://bqw.yuanzhike.top

free -h;  ps aux | grep nginx
来源：http://sol.c1oappe.top

[R64] 结束进程
来源：http://fra.birdmap.top

kill -9 $(pgrep -f app.py)
来源：http://lor.ctjpmb.com

[R65] 查看端口占用
来源：http://xag.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gcm.feifeiyinyue.top

[R66] 定时任务
来源：http://eft.fehbvm.com

crontab -e;  crontab -l
来源：http://qli.tarul.cn

[R67] 生成随机十六进制串
来源：http://rxj.meibo888.top

openssl rand -hex 16
来源：http://kzl.pycfn.com

[R68] 计算文件校验值
来源：http://pam.hesvh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ozo.jyoumei.cn

[R69] 生成随机密码
来源：http://vet.sweek.top

head -c 16 /dev/urandom | base64
来源：http://acp.shangyingyoupin.top

[R70] 时间戳与互转
来源：http://jct.nwbrower.top

date +%s;  date -d @1700000000
来源：http://qnv.yuxming.cn

[R71] 日期格式化
来源：http://ber.fanxiaobao.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://wyn.xinyue.icu

[R72] 等待端口就绪
来源：http://axw.zycfv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ekk.hcnkem.com

[R73] 分割大日志
来源：http://fwf.sweek.top

split -l 1000 big.log part_
来源：http://dwm.cucudq.cn

[R74] 批量重命名
来源：http://ehr.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dod.zdqjudy.top

[R75] 导出环境变量
来源：http://lxf.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://wfo.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://snz.sweek.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vwy.zhoulong.xyz

[R77] 读取用户输入
来源：http://chp.hfpthk.cn

read -rp "请输入: " ans
来源：http://okz.hnxiangtu.top

[R78] 交互式菜单
来源：http://xzb.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://iux.tarul.cn

[R79] 解析命令行选项
来源：http://lly.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ppc.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://hvc.316326.xyz

time ./run.sh
来源：http://uwu.pengpengdd.cyou

================================================================================
来源：http://gme.gotoacloud.top

S. C / C++ 专题
来源：http://kpr.zhoulong.xyz

================================================================================
来源：http://tlq.yonumen.top

[S01] C：Hello World
来源：http://kqv.nanxuanxn.top

#include <stdio.h>
来源：http://yas.hongshengwenyu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ijd.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://llx.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://nqk.hnxiangtu.top

[S03] C：读入整数
来源：http://bvi.fehbvm.com

int x; scanf("%d", &x);
来源：http://xes.cqqwz.cn

[S04] C：字符串复制
来源：http://kjv.smart0.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://umr.yj20258888.top

[S05] C：字符串长度
来源：http://lym.tanke756.top

strlen(s)
来源：http://uao.sxryk.cn

[S06] C：字符串比较
来源：http://yrb.316326.xyz

strcmp(a, b) == 0
来源：http://pze.yongpay.top

[S07] C：数组遍历求和
来源：http://vzw.zhaomingkeji.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jbf.andypj.xyz

[S08] C：动态内存分配与释放
来源：http://utx.feifeiyinyue.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rxm.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://zpy.fengsongda.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ydf.bbcook.cn

[S10] C：指针与解引用
来源：http://ncl.yongpay.top

int *p = &a;  *p = 5;
来源：http://bwx.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://eji.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://mwm.hnxiangtu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ytt.ywan-chungtsiang.top

fclose(f);
来源：http://fzp.yueranfly.top

[S12] C：写文件
来源：http://haj.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://unp.daria6918.cn

[S13] C：宏定义
来源：http://voa.shuidangran.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bwg.sweek.top

[S14] C：枚举
来源：http://sol.zdbjq.cn


<!-- 参考信息 -->