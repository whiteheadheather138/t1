代发 wailian999

[Q48] CTE 公用表表达式
来源：http://ztf.kuanghao11.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://igp.bbcook.cn

SELECT * FROM t WHERE c > 5;
来源：http://rfn.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://ffw.bjfxy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jiy.xingfuxueyuan.xyz

[Q50] 批量更新
来源：http://zkp.tanke756.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fse.uphjek.com

[Q51] 用子查询更新
来源：http://usf.hysaishi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://noh.cashguo.top

[Q52] 删除指定行
来源：http://bla.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://ajg.snrcjt.cn

[Q53] 按条件删除
来源：http://daz.feifeiyinyue.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://asz.nanxuanxn.top

[Q54] 清空表
来源：http://pil.zhijiandao.cn

TRUNCATE TABLE logs;
来源：http://mrj.0kj1m.cn

[Q55] 排名（并列占位）
来源：http://zeb.ppjwa.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vaz.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://urb.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://irg.yangfankeji.com

[Q57] 行号
来源：http://hfj.yongpay.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://imm.gzhubu.top

[Q58] 累计求和
来源：http://tid.yj202588.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://znx.yanxiufei.cn

[Q59] 分组内累计
来源：http://hcp.yanxiufei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://btc.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://qxj.quarkkingdee.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vcg.yangfankeji.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://aga.ydjk.org.cn

[Q61] 移动平均
来源：http://zjn.jyoumei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hjb.hysaishi.cn

[Q62] 分组占比
来源：http://leo.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ckv.yj20258.top

[Q63] 开启事务
来源：http://uim.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://csj.cqqwz.cn

[Q64] 提交事务
来源：http://vge.shangyingyoupin.top

COMMIT;
来源：http://rjp.yvedp.cn

[Q65] 回滚事务
来源：http://reo.svipenyu.cn

ROLLBACK;
来源：http://pzj.zhiwuduotai.top

[Q66] 行锁查询
来源：http://xrp.hongshengwenyu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vcq.hnqzz.top

[Q67] 设置隔离级别
来源：http://lxv.hfpthk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sth.ybcxt.top

[Q68] 保存点
来源：http://iwk.yj20258.top

SAVEPOINT sp1;
来源：http://fgz.feifeiyinyue.top

ROLLBACK TO sp1;
来源：http://dqo.chenzaomai.com

[Q69] 查看执行计划
来源：http://fgc.ctjpmb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://okc.c1oappe.top

[Q70] 更新统计信息
来源：http://zal.yuanzhike.top

ANALYZE TABLE users;
来源：http://tyw.gzhubu.top

[Q71] 查看建表语句
来源：http://ggb.gogol.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wus.havefunace.top

[Q72] 查看索引
来源：http://hfu.dianchejie.cn

SHOW INDEX FROM users;
来源：http://jsd.dianchejie.cn

[Q73] 查看表状态
来源：http://mnc.xingfuxueyuan.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://rbb.xuetiantiany.cn

[Q74] 强制使用索引
来源：http://upg.yangfankeji.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kkt.zdbjq.cn

[Q75] 日期格式化
来源：http://yfd.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://htg.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nej.yueranfly.top

[Q76] 按天统计
来源：http://nqd.pengpengdd.cyou

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tmj.xingfuxueyuan.xyz

[Q77] 时间加减
来源：http://ldu.uphjek.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dau.zhiwuduotai.top

[Q78] 当前时间
来源：http://qzs.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ltu.tianlin.xyz

[Q79] 字符串拼接
来源：http://itm.fehbvm.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nfk.chenjidiqi.icu

[Q80] 字符串截取
来源：http://qfk.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cme.ybcxt.top

[Q81] 字符串替换
来源：http://bfl.jiagoushi.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xok.yj202588.top

[Q82] 字符长度与字节长度
来源：http://tci.gogol.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ovd.guowangkeji.top

[Q83] 大小写转换
来源：http://whl.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yzz.yfazqb.com

[Q84] 去除首尾空格
来源：http://ijh.jiagoushi.top

SELECT TRIM(name) FROM users;
来源：http://zmd.birdmap.top

[Q85] 数值取整
来源：http://mhl.zdbjq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hym.zhiwuduotai.top

[Q86] 读取 JSON 字段
来源：http://usm.sxryk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qnx.haohaochexian.top

[Q87] JSON 字段做条件
来源：http://opu.xingfuxueyuan.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bxk.ctjpmb.com

[Q88] 行转列（条件聚合）
来源：http://mwe.ydjk.org.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nfx.pycfn.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pdq.cheryme.top

[Q89] 判断表是否存在
来源：http://hxl.fehbvm.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ddj.fzhhl.top

[Q90] 生成序号列
来源：http://ouh.redwolf501.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wsv.iojbl.cn

================================================================================
来源：http://htk.zhoulong.xyz

R. Bash 专题
来源：http://eet.chenzaomai.com

================================================================================
来源：http://fhz.yongpay.top

[R01] shebang 与严格模式
来源：http://jtn.epnwcf.com

#!/usr/bin/env bash
来源：http://dbz.tanke756.top

set -euo pipefail
来源：http://prj.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://iiv.guannengcc.top

name="Tom"; echo "$name"
来源：http://bes.bbcook.cn

[R03] 只读变量
来源：http://kby.vqdsnc.cn

readonly PI=3.14
来源：http://awf.aibaodan.cn

[R04] 位置参数
来源：http://ovb.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://syu.ydjk.org.cn

[R05] 参数默认值
来源：http://sve.gaohongyu789.top

name="${1:-default}"
来源：http://urz.jinqigufen.top

[R06] 判断命令是否存在
来源：http://wix.fengsongda.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lyp.kuanghao11.cn

[R07] if 判断文件
来源：http://kcc.52xcode.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dhr.feifeiyinyue.top

[R08] 数值比较
来源：http://nxj.yanxiufei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gll.0kj1m.cn

[R09] 字符串比较
来源：http://etc.shanyushiyangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kng.daxiang520.top

[R10] 正则匹配
来源：http://cmo.ywan-chungtsiang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cbu.shzxlz.cn

[R11] case 多分支
来源：http://bpm.aibaodan.cn

case "$1" in
来源：http://urk.fktsv.cn

start) echo "启动" ;;
来源：http://gyj.shuidangran.top

stop)  echo "停止" ;;
来源：http://gfo.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://adt.shuidangran.top

esac
来源：http://fim.cqqwz.cn

[R12] for 遍历文件
来源：http://amu.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://oua.tanke756.top

[R13] for 计数循环
来源：http://pzb.tian-w.cn

for i in {1..10}; do echo "$i"; done
来源：http://khm.xingfuxueyuan.xyz

[R14] C 风格 for
来源：http://xpw.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://saj.gotoacloud.top

[R15] while 逐行读文件
来源：http://kri.chenzaomai.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cts.sufxvd.cn

[R16] until 等待条件
来源：http://ltd.fktsv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fjt.yfazqb.com

[R17] 数组定义与取值
来源：http://uyo.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://dne.mhx1999.top

[R18] 遍历数组
来源：http://oxs.zdqjudy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ujw.shzxlz.cn

[R19] 数组长度
来源：http://dgw.hongshengwenyu.top

echo "${#arr[@]}"
来源：http://cww.nwbrower.top

[R20] 关联数组（字典）
来源：http://ljt.0kj1m.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qdt.gaohongyu789.top

[R21] 字符串长度
来源：http://myc.ywan-chungtsiang.top

echo "${#s}"
来源：http://yfz.9152youxi.cn

[R22] 截取子串
来源：http://rtd.daria6918.cn

echo "${s:0:5}"
来源：http://pma.xinyue.icu

[R23] 字符串替换
来源：http://apy.zhengqikj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kbk.yuanzhike.top

[R24] 大小写转换
来源：http://bvr.shzxlz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tpf.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://qzc.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bms.tianlin.xyz

[R26] 命令替换
来源：http://kor.yangfankeji.com

now=$(date +%F); echo "$now"
来源：http://fcx.snrcjt.cn

[R27] 算术展开
来源：http://zkn.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://hrb.vehdjk.com

[R28] 浮点运算
来源：http://hpe.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://prx.xinyue.icu

[R29] 定义函数
来源：http://pkx.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mhu.ivvv.top

[R30] 函数返回状态码
来源：http://oxa.gotoacloud.top

f() { return 0; }; f || echo "失败了"
来源：http://vks.gogol.net.cn

[R31] 局部变量
来源：http://pst.haohaochexian.top

f() { local x=1; echo "$x"; }
来源：http://jlb.xinyue.icu

[R32] 参数个数校验
来源：http://xqz.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hhk.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://bah.sjlbkw.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tvo.52xcode.cn

[R34] 退出时清理
来源：http://rue.hnxiangtu.top

trap 'rm -f "$tmp"' EXIT
来源：http://avu.gzhubu.top

[R35] 后台执行并等待
来源：http://lqf.hysaishi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uug.svipenyu.cn

[R36] 并发执行多个任务
来源：http://koo.daxiang520.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://slw.daxiang520.top

[R37] 把输出赋给变量
来源：http://zqq.sysykeji.top

files=$(ls -1)
来源：http://dxs.ctjpmb.com

[R38] 管道串联
来源：http://gbc.yj20258.top

cat a.txt | grep -i error | wc -l
来源：http://ndi.yvedp.cn

[R39] 重定向标准输出与错误
来源：http://urg.gogol.net.cn

cmd > out.log 2>&1
来源：http://fkd.jlsjyb.cn

[R40] 追加写日志
来源：http://fbs.sufxvd.cn

echo "log" >> out.log
来源：http://deq.aibaodan.cn

[R41] 丢弃输出
来源：http://dif.mhx1999.top

cmd >/dev/null 2>&1
来源：http://tdu.iojbl.cn

[R42] 输入重定向
来源：http://gdt.yj20258888.top

wc -l < a.txt
来源：http://kco.zdbjq.cn

[R43] 按名字查找文件
来源：http://icp.hammf.cn

find . -name "*.log" -type f
来源：http://cbi.ehwqpu.com

[R44] 按修改时间查找
来源：http://vag.hammf.cn

find . -mtime -7 -type f
来源：http://lth.hesvh.cn

[R45] 批量删除
来源：http://xbk.dashuyun.cn

find . -name "*.tmp" -delete
来源：http://ywc.ybcxt.top

[R46] 递归替换文件内容
来源：http://his.ydjk.org.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ywl.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://fzo.jinqigfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://ntr.yj202588.top

[R48] awk 取指定列
来源：http://fwg.hywenlv.cn

awk '{print $1, $3}' a.txt
来源：http://hyi.tianlin.xyz

[R49] awk 带条件
来源：http://tbm.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ydp.hongshengwenyu.top

[R50] awk 求和
来源：http://cxw.kuanghao11.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wju.c1oappe.top

[R51] 排序去重取前几
来源：http://leh.ybcxt.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xhe.shzxlz.cn

[R52] 统计行数
来源：http://mub.wangdashe.top

wc -l a.txt
来源：http://enc.yangfankeji.com

[R53] 查看文件头与实时尾
来源：http://tbg.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ugt.svipenyu.cn

[R54] 比较两个文件
来源：http://khr.yangfankeji.com

diff a.txt b.txt
来源：http://spz.snrcjt.cn

[R55] 压缩与解压
来源：http://gjl.zhaomingkeji.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lag.ywan-chungtsiang.top

[R56] 远程拷贝
来源：http://www.chenzaomai.com

scp file user@host:/path/
来源：http://ezd.chenzaomai.com

[R57] 远程执行命令
来源：http://cqv.0kj1m.cn

ssh user@host 'uptime'
来源：http://jsp.smart0.xyz

[R58] 下载文件
来源：http://enc.hfpthk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nft.tian-w.cn

[R59] 发 POST JSON
来源：http://jkw.52xcode.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fpm.0kj1m.cn

[R60] 只看 HTTP 状态码
来源：http://cqu.hammf.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ygn.pengpengdd.cyou

[R61] 磁盘占用
来源：http://kus.ydzc1.top

df -h;  du -sh *
来源：http://fid.gaohongyu789.top

[R62] 找最占空间的文件
来源：http://jme.andypj.xyz

du -ah . | sort -rh | head -10
来源：http://rvs.xuanzx.com

[R63] 内存与进程
来源：http://icr.hesvh.cn

free -h;  ps aux | grep nginx
来源：http://wfg.fengsongda.top

[R64] 结束进程
来源：http://ybb.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://ezy.hywenlv.cn

[R65] 查看端口占用
来源：http://bur.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zim.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://hvu.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://psp.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://jck.havefunace.top

openssl rand -hex 16
来源：http://ttf.daria6918.cn

[R68] 计算文件校验值
来源：http://veb.cashguo.top

sha256sum a.txt;  md5sum a.txt
来源：http://gar.jqgufenzy.top

[R69] 生成随机密码
来源：http://amn.guowangkeji.top

head -c 16 /dev/urandom | base64
来源：http://pid.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://yxm.jqgufenzy.top

date +%s;  date -d @1700000000
来源：http://nnj.quarkkingdee.top

[R71] 日期格式化
来源：http://vra.wangshuangyany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nlj.jlsjyb.cn

[R72] 等待端口就绪
来源：http://xbw.zycfv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vgn.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://ive.gzhubu.top

split -l 1000 big.log part_
来源：http://kor.sysykeji.top

[R74] 批量重命名
来源：http://qnd.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://arq.yangfankeji.com

[R75] 导出环境变量
来源：http://cnt.aizwys.cn

export PATH="$HOME/bin:$PATH"
来源：http://fwt.xziqi.cn

[R76] 使用临时文件
来源：http://xpw.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sba.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://dkb.316326.xyz

read -rp "请输入: " ans
来源：http://sxa.0kj1m.cn

[R78] 交互式菜单
来源：http://rnw.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wux.jqgfzy.top

[R79] 解析命令行选项
来源：http://iqt.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fyy.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://kie.smart0.xyz

time ./run.sh
来源：http://vhf.hammf.cn

================================================================================
来源：http://mbz.xylfe.cn

S. C / C++ 专题
来源：http://wfw.gotoacloud.top

================================================================================
来源：http://lcr.hysaishi.cn

[S01] C：Hello World
来源：http://prv.ppjwa.cn

#include <stdio.h>
来源：http://bvc.sweek.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qsa.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://cst.yanxiufei.cn

int a = 10; printf("%d\n", a);
来源：http://dyz.dianchejie.cn

[S03] C：读入整数
来源：http://fnx.sweek.top

int x; scanf("%d", &x);
来源：http://wrn.guannengcc.top

[S04] C：字符串复制
来源：http://nsq.sysykeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://gvg.pengpengdd.cyou

[S05] C：字符串长度
来源：http://dqh.hnqzz.top

strlen(s)
来源：http://xwy.gotoacloud.top

[S06] C：字符串比较
来源：http://gkh.tianlin.xyz

strcmp(a, b) == 0
来源：http://pof.tianlin.xyz

[S07] C：数组遍历求和
来源：http://pnb.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bvr.hammf.cn

[S08] C：动态内存分配与释放
来源：http://rpv.sufxvd.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bcv.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://jep.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dnx.pycfn.com

[S10] C：指针与解引用
来源：http://zua.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://jec.ywan-chungtsiang.top

[S11] C：逐行读文件
来源：http://aiu.fanxiaobao.xyz

FILE *f = fopen("a.txt", "r");
来源：http://wdx.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qrb.zhiwuduotai.top

fclose(f);
来源：http://bif.cashguo.top

[S12] C：写文件
来源：http://hsu.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yxy.jiagoushi.top

[S13] C：宏定义
来源：http://thw.iojbl.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xnw.yfazqb.com

[S14] C：枚举
来源：http://hac.aizwys.cn

enum Color { RED, GREEN, BLUE };
来源：http://mis.shanyushiyangtech.top

[S15] C：类型转换
来源：http://iym.xziqi.cn

(double) a / b
来源：http://fii.mhx1999.top

[S16] C：位操作置位
来源：http://hsn.tarul.cn

x |= (1 << 3);
来源：http://omf.yonumen.top

[S17] C：安全拼接字符串
来源：http://zba.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ddo.tianlin.xyz

[S18] C：命令行参数
来源：http://tgs.hysaishi.cn


<!-- 参考信息 -->