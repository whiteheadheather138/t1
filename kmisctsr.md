代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kne.jinghuilouyu.cn

[Q50] 批量更新
来源：http://ptf.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://inx.ybcxt.top

[Q51] 用子查询更新
来源：http://oxi.xinyue.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lks.zdbjq.cn

[Q52] 删除指定行
来源：http://kzs.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://raq.fengsongda.top

[Q53] 按条件删除
来源：http://txn.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dxp.hongshengwenyu.top

[Q54] 清空表
来源：http://qfw.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://uyq.yj20258.top

[Q55] 排名（并列占位）
来源：http://fli.pengpengdd.cyou

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hqa.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://yds.jqgfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mvy.fktsv.cn

[Q57] 行号
来源：http://hqh.chenzaomai.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jgj.yuanzhike.top

[Q58] 累计求和
来源：http://dce.jqgufenzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://edr.redwolf501.top

[Q59] 分组内累计
来源：http://vvb.haohaochexian.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rui.9152youxi.cn

[Q60] 取上一行 / 下一行
来源：http://yez.yonumen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uxo.shanyushiyangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kpl.shzxlz.cn

[Q61] 移动平均
来源：http://uiw.hesvh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://psb.xuetiantiany.cn

[Q62] 分组占比
来源：http://nog.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fzn.ctjpmb.com

[Q63] 开启事务
来源：http://awf.sweek.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kfz.bbcook.cn

[Q64] 提交事务
来源：http://xqi.gaohongyu789.top

COMMIT;
来源：http://gpz.52xcode.cn

[Q65] 回滚事务
来源：http://fvh.shanyushiyangkeji.top

ROLLBACK;
来源：http://vqx.hnxiangtu.top

[Q66] 行锁查询
来源：http://cwp.zhoulong.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://orz.hnxiangtu.top

[Q67] 设置隔离级别
来源：http://uxw.cqqwz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kwb.wangshuangyany.cn

[Q68] 保存点
来源：http://kbn.zdbjq.cn

SAVEPOINT sp1;
来源：http://fmf.yj20258888.top

ROLLBACK TO sp1;
来源：http://eka.jyoumei.cn

[Q69] 查看执行计划
来源：http://ogh.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nve.andypj.xyz

[Q70] 更新统计信息
来源：http://vxh.cucudq.cn

ANALYZE TABLE users;
来源：http://aht.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://trx.chenjidiqi.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nha.nwbrower.top

[Q72] 查看索引
来源：http://swx.feifeiyinyue.top

SHOW INDEX FROM users;
来源：http://wzo.52xcode.cn

[Q73] 查看表状态
来源：http://wbt.zhiwuduotai.top

SHOW TABLE STATUS LIKE 'users';
来源：http://phg.andypj.xyz

[Q74] 强制使用索引
来源：http://jke.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ugb.fktsv.cn

[Q75] 日期格式化
来源：http://ccm.gogol.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xcm.zhongyouzk.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nda.hcnkem.com

[Q76] 按天统计
来源：http://yff.hnqzz.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lfe.yueranfly.top

[Q77] 时间加减
来源：http://occ.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xsc.bbcook.cn

[Q78] 当前时间
来源：http://mtm.daria6918.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hla.shzxlz.cn

[Q79] 字符串拼接
来源：http://sgr.yvedp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xhe.cqqwz.cn

[Q80] 字符串截取
来源：http://tsf.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ozr.zhijiandao.cn

[Q81] 字符串替换
来源：http://rpz.zycfv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://axj.quarkkingdee.top

[Q82] 字符长度与字节长度
来源：http://orp.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yai.chenjidiqi.icu

[Q83] 大小写转换
来源：http://ykw.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uhx.guowangkeji.top

[Q84] 去除首尾空格
来源：http://fzl.cheryme.top

SELECT TRIM(name) FROM users;
来源：http://gmy.hfpthk.cn

[Q85] 数值取整
来源：http://piu.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pkz.fanxiaobao.xyz

[Q86] 读取 JSON 字段
来源：http://cfe.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tlx.nanxuanxn.top

[Q87] JSON 字段做条件
来源：http://ydw.andypj.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://imy.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://xns.ydjk.org.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hew.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fau.andypj.xyz

[Q89] 判断表是否存在
来源：http://ufb.meibo888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kem.tanke756.top

[Q90] 生成序号列
来源：http://xzn.hongshengwenyu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jcs.hammf.cn

================================================================================
来源：http://ici.snrcjt.cn

R. Bash 专题
来源：http://xge.yfazqb.com

================================================================================
来源：http://tak.ywan-chungtsiang.top

[R01] shebang 与严格模式
来源：http://etr.daxiang520.top

#!/usr/bin/env bash
来源：http://ryh.shangyingyoupin.top

set -euo pipefail
来源：http://dae.yonumen.top

[R02] 变量赋值与使用
来源：http://jtd.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://epk.iojbl.cn

[R03] 只读变量
来源：http://pdu.9152youxi.cn

readonly PI=3.14
来源：http://flf.nanxuanxn.top

[R04] 位置参数
来源：http://yzq.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zcu.fanxiaobao.xyz

[R05] 参数默认值
来源：http://txx.yueranfly.top

name="${1:-default}"
来源：http://jmr.yuanzhike.top

[R06] 判断命令是否存在
来源：http://ejs.nanxuanxn.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dza.fktsv.cn

[R07] if 判断文件
来源：http://arq.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vyb.cheryme.top

[R08] 数值比较
来源：http://hig.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://pfv.chenzaomai.com

[R09] 字符串比较
来源：http://vgb.cucudq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aya.feifeiyinyue.top

[R10] 正则匹配
来源：http://imj.yj20258888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qow.fktsv.cn

[R11] case 多分支
来源：http://nmt.quarkkingdee.top

case "$1" in
来源：http://ceu.shanyushiyangkeji.top

start) echo "启动" ;;
来源：http://igw.xziqi.cn

stop)  echo "停止" ;;
来源：http://mip.havefunace.top

*)     echo "未知命令" ;;
来源：http://jra.svipenyu.cn

esac
来源：http://vgj.hongshengwenyu.top

[R12] for 遍历文件
来源：http://tre.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://osm.wangshuangyany.cn

[R13] for 计数循环
来源：http://kgf.jinyuanbaomall.cn

for i in {1..10}; do echo "$i"; done
来源：http://mvf.vqdsnc.cn

[R14] C 风格 for
来源：http://ffj.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fkn.sysykeji.top

[R15] while 逐行读文件
来源：http://skk.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://usa.yuxming.cn

[R16] until 等待条件
来源：http://phx.sxryk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gxr.quarkkingdee.top

[R17] 数组定义与取值
来源：http://zel.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://eup.jlsjyb.cn

[R18] 遍历数组
来源：http://wur.ybcxt.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rxy.jianghu66.top

[R19] 数组长度
来源：http://qot.fengsongda.top

echo "${#arr[@]}"
来源：http://ebc.zhixingplan.top

[R20] 关联数组（字典）
来源：http://lsp.fehbvm.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://noo.jinqigfzy.top

[R21] 字符串长度
来源：http://fje.zhongyouzk.top

echo "${#s}"
来源：http://ycp.redwolf501.top

[R22] 截取子串
来源：http://ach.jianghu66.top

echo "${s:0:5}"
来源：http://bex.mhx1999.top

[R23] 字符串替换
来源：http://upj.hysaishi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xtu.nanxuanxn.top

[R24] 大小写转换
来源：http://ycn.xinyue.icu

echo "${s^^}"; echo "${s,,}"
来源：http://xwk.pengpengdd.cyou

[R25] 去后缀 / 去前缀
来源：http://grz.guannengcc.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tpm.sufxvd.cn

[R26] 命令替换
来源：http://rvl.fehbvm.com

now=$(date +%F); echo "$now"
来源：http://dad.sysykeji.top

[R27] 算术展开
来源：http://yix.yonumen.top

echo $((1 + 2 * 3))
来源：http://npr.nwbrower.top

[R28] 浮点运算
来源：http://eym.hongshengwenyu.top

echo "scale=2; 10/3" | bc
来源：http://axl.epnwcf.com

[R29] 定义函数
来源：http://ynr.gogol.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uuf.hesvh.cn

[R30] 函数返回状态码
来源：http://ouf.smart0.xyz

f() { return 0; }; f || echo "失败了"
来源：http://ori.smart0.xyz

[R31] 局部变量
来源：http://csu.shangyingyoupin.top

f() { local x=1; echo "$x"; }
来源：http://jrm.sufxvd.cn

[R32] 参数个数校验
来源：http://udq.ydjk.org.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mxf.gaohongyu789.top

[R33] 捕获错误并提示行号
来源：http://edb.svipenyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mqh.sysykeji.top

[R34] 退出时清理
来源：http://pal.zhijiandao.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sba.uphjek.com

[R35] 后台执行并等待
来源：http://mjf.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pjo.chenzaomai.com

[R36] 并发执行多个任务
来源：http://frq.jqgufenzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qcc.jinghuilouyu.cn

[R37] 把输出赋给变量
来源：http://xpo.hnqzz.top

files=$(ls -1)
来源：http://zkk.ywan-chungtsiang.top

[R38] 管道串联
来源：http://fvi.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://mdc.guowangkeji.top

[R39] 重定向标准输出与错误
来源：http://vht.yfazqb.com

cmd > out.log 2>&1
来源：http://efj.jlsjyb.cn

[R40] 追加写日志
来源：http://eld.havefunace.top

echo "log" >> out.log
来源：http://znr.kuanghao11.cn

[R41] 丢弃输出
来源：http://evn.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://nid.dashuyun.cn

[R42] 输入重定向
来源：http://lmw.yj20258888.top

wc -l < a.txt
来源：http://apf.xylfe.cn

[R43] 按名字查找文件
来源：http://jzo.fktsv.cn

find . -name "*.log" -type f
来源：http://fhx.shzxlz.cn

[R44] 按修改时间查找
来源：http://ndl.jianghu66.top

find . -mtime -7 -type f
来源：http://fmd.hnqzz.top

[R45] 批量删除
来源：http://ukr.jinyuanbaomall.cn

find . -name "*.tmp" -delete
来源：http://wfv.smart0.xyz

[R46] 递归替换文件内容
来源：http://pmx.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vkh.316326.xyz

[R47] sed 单行替换
来源：http://cbv.yvedp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cvb.aizwys.cn

[R48] awk 取指定列
来源：http://jlo.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://svt.ppjwa.cn

[R49] awk 带条件
来源：http://vkt.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tbb.aizwys.cn

[R50] awk 求和
来源：http://gyk.fanxiaobao.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://vws.c1oappe.top

[R51] 排序去重取前几
来源：http://wxt.zhaomingkeji.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://ens.cucudq.cn

[R52] 统计行数
来源：http://jij.jlsjyb.cn

wc -l a.txt
来源：http://zfx.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://vyp.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fez.sweek.top

[R54] 比较两个文件
来源：http://nai.vqdsnc.cn

diff a.txt b.txt
来源：http://fqe.jiagoushi.top

[R55] 压缩与解压
来源：http://smu.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hrm.gaohongyu789.top

[R56] 远程拷贝
来源：http://pwi.pycfn.com

scp file user@host:/path/
来源：http://rfb.guannengcc.top

[R57] 远程执行命令
来源：http://eqf.ybcxt.top

ssh user@host 'uptime'
来源：http://euw.jinghuilouyu.cn

[R58] 下载文件
来源：http://txy.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tjv.kuanghao11.cn

[R59] 发 POST JSON
来源：http://ecx.shzxlz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qcx.hfpthk.cn

[R60] 只看 HTTP 状态码
来源：http://lbg.cdnleiting.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mfm.ywan-chungtsiang.top

[R61] 磁盘占用
来源：http://bpd.epnwcf.com

df -h;  du -sh *
来源：http://ycy.yj20258.top

[R62] 找最占空间的文件
来源：http://pql.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://jgp.yj20258888.top

[R63] 内存与进程
来源：http://bvf.zdbjq.cn

free -h;  ps aux | grep nginx
来源：http://tjm.yonumen.top

[R64] 结束进程
来源：http://thi.nwbrower.top

kill -9 $(pgrep -f app.py)
来源：http://mpr.jqgufenzy.top

[R65] 查看端口占用
来源：http://bdc.52xcode.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uqj.ppjwa.cn

[R66] 定时任务
来源：http://mlr.tarul.cn

crontab -e;  crontab -l
来源：http://syb.redwolf501.top

[R67] 生成随机十六进制串
来源：http://hjj.aizwys.cn

openssl rand -hex 16
来源：http://ovx.yongpay.top

[R68] 计算文件校验值
来源：http://tfv.mhx1999.top

sha256sum a.txt;  md5sum a.txt
来源：http://hnz.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://ddc.mhx1999.top

head -c 16 /dev/urandom | base64
来源：http://pav.xziqi.cn

[R70] 时间戳与互转
来源：http://lxc.zhijiandao.cn

date +%s;  date -d @1700000000
来源：http://ghg.gogol.net.cn

[R71] 日期格式化
来源：http://mqx.yvedp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tez.xylfe.cn

[R72] 等待端口就绪
来源：http://zyk.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dlc.hywenlv.cn

[R73] 分割大日志
来源：http://twq.xingfuxueyuan.xyz

split -l 1000 big.log part_
来源：http://kjh.yongpay.top

[R74] 批量重命名
来源：http://xay.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kpx.aibaodan.cn

[R75] 导出环境变量
来源：http://ddy.smart0.xyz

export PATH="$HOME/bin:$PATH"
来源：http://pcw.fengsongda.top

[R76] 使用临时文件
来源：http://fde.cucudq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mol.wangshuangyany.cn

[R77] 读取用户输入
来源：http://irc.jqgufenzy.top

read -rp "请输入: " ans
来源：http://srq.fengsongda.top

[R78] 交互式菜单
来源：http://bml.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://stw.mhx1999.top

[R79] 解析命令行选项
来源：http://rxh.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uqi.yongpay.top

[R80] 查看脚本执行耗时
来源：http://uni.sjlbkw.cn

time ./run.sh
来源：http://wxl.hesvh.cn

================================================================================
来源：http://dvk.cqqwz.cn

S. C / C++ 专题
来源：http://mgs.tanke756.top

================================================================================
来源：http://ikk.ppjwa.cn

[S01] C：Hello World
来源：http://fck.shangyingyoupin.top

#include <stdio.h>
来源：http://gfm.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://rfj.yvedp.cn

[S02] C：变量与格式化输出
来源：http://gwr.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://ktl.gogol.net.cn

[S03] C：读入整数
来源：http://cpj.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://lyf.shanyushiyangkeji.top

[S04] C：字符串复制
来源：http://lfo.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://wug.yfazqb.com

[S05] C：字符串长度
来源：http://pfw.hysaishi.cn

strlen(s)
来源：http://zlg.zdbjq.cn

[S06] C：字符串比较
来源：http://ndz.hesvh.cn

strcmp(a, b) == 0
来源：http://jap.jianghu66.top

[S07] C：数组遍历求和
来源：http://sdj.jqgfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jny.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://mgv.quarkkingdee.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xuf.quarkkingdee.top

[S09] C：结构体定义与初始化
来源：http://nyx.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ilj.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://kun.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://tpd.guannengcc.top

[S11] C：逐行读文件
来源：http://rcc.shzxlz.cn

FILE *f = fopen("a.txt", "r");
来源：http://vpj.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ymf.dashuyun.cn

fclose(f);
来源：http://ekr.havefunace.top

[S12] C：写文件
来源：http://god.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xuc.wangdashe.top

[S13] C：宏定义
来源：http://dme.yvedp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zvu.fzhhl.top

[S14] C：枚举
来源：http://pky.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://let.ehwqpu.com

[S15] C：类型转换
来源：http://pnv.yj20258.top

(double) a / b
来源：http://zbx.yvedp.cn

[S16] C：位操作置位
来源：http://ygl.52xcode.cn

x |= (1 << 3);
来源：http://lua.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://pul.zhiwuduotai.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ykt.smart0.xyz

[S18] C：命令行参数
来源：http://qfp.jianghu66.top

int main(int argc, char **argv)
来源：http://nzd.9152youxi.cn

[S19] C：快速排序
来源：http://ede.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://xle.yongpay.top

[S20] C：二分查找
来源：http://gfk.yuanzhike.top


<!-- 参考信息 -->