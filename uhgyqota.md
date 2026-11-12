代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yvf.guowangkeji.top

[Q50] 批量更新
来源：http://zct.daxiang520.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zgx.hammf.cn

[Q51] 用子查询更新
来源：http://mpa.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bjw.yonumen.top

[Q52] 删除指定行
来源：http://gxb.jinqigfzy.top

DELETE FROM users WHERE id = 10;
来源：http://owr.yvedp.cn

[Q53] 按条件删除
来源：http://bnn.hammf.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sjy.hfpthk.cn

[Q54] 清空表
来源：http://hzz.xuanzx.com

TRUNCATE TABLE logs;
来源：http://sni.0kj1m.cn

[Q55] 排名（并列占位）
来源：http://wiq.shanyushiyangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rkw.shangyingyoupin.top

[Q56] 密集排名（并列不占位）
来源：http://qld.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xdn.epnwcf.com

[Q57] 行号
来源：http://vjt.sxryk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yjy.andypj.xyz

[Q58] 累计求和
来源：http://gmy.guannengcc.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dxq.gaohongyu789.top

[Q59] 分组内累计
来源：http://mea.gogol.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wrr.zhoulong.xyz

[Q60] 取上一行 / 下一行
来源：http://rkr.hesvh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zyj.jinqigfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cvp.gogol.net.cn

[Q61] 移动平均
来源：http://bse.hysaishi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rxk.yueranfly.top

[Q62] 分组占比
来源：http://yox.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uzz.aibaodan.cn

[Q63] 开启事务
来源：http://rnh.xylfe.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rve.ctjpmb.com

[Q64] 提交事务
来源：http://vck.yongpay.top

COMMIT;
来源：http://zlg.jianghu66.top

[Q65] 回滚事务
来源：http://kal.yuxming.cn

ROLLBACK;
来源：http://grr.sufxvd.cn

[Q66] 行锁查询
来源：http://dyt.quarkkingdee.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zbo.bbcook.cn

[Q67] 设置隔离级别
来源：http://bga.ppjwa.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yxc.sjlbkw.cn

[Q68] 保存点
来源：http://mlr.fktsv.cn

SAVEPOINT sp1;
来源：http://esz.hysaishi.cn

ROLLBACK TO sp1;
来源：http://lbg.mhx1999.top

[Q69] 查看执行计划
来源：http://vic.pengpengdd.cyou

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xvw.yuanzhike.top

[Q70] 更新统计信息
来源：http://zda.hfpthk.cn

ANALYZE TABLE users;
来源：http://zlx.dashuyun.cn

[Q71] 查看建表语句
来源：http://ies.jiagoushi.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hnz.quarkkingdee.top

[Q72] 查看索引
来源：http://sqz.haohaochexian.top

SHOW INDEX FROM users;
来源：http://ibd.ywan-chungtsiang.top

[Q73] 查看表状态
来源：http://pvz.fzhhl.top

SHOW TABLE STATUS LIKE 'users';
来源：http://aqt.shuidangran.top

[Q74] 强制使用索引
来源：http://pqk.zhoulong.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tue.jinyuanbaomall.cn

[Q75] 日期格式化
来源：http://sfz.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dwt.chenjidiqi.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qcl.chenjidiqi.icu

[Q76] 按天统计
来源：http://mzp.cheryme.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fjh.quarkkingdee.top

[Q77] 时间加减
来源：http://zxm.dianchejie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://axz.birdmap.top

[Q78] 当前时间
来源：http://gbk.hnqzz.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xuq.tarul.cn

[Q79] 字符串拼接
来源：http://dph.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://htg.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://aow.sjlbkw.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://auv.pycfn.com

[Q81] 字符串替换
来源：http://tsu.cashguo.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hri.gogol.net.cn

[Q82] 字符长度与字节长度
来源：http://ain.yfazqb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xhf.ydzc1.top

[Q83] 大小写转换
来源：http://uvt.hcnkem.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uqn.ctjpmb.com

[Q84] 去除首尾空格
来源：http://jgs.sweek.top

SELECT TRIM(name) FROM users;
来源：http://soa.zhongyouzk.top

[Q85] 数值取整
来源：http://krs.fengsongda.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xxa.chenjidiqi.icu

[Q86] 读取 JSON 字段
来源：http://jtu.tianlin.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cuk.jqgfzy.top

[Q87] JSON 字段做条件
来源：http://fjm.pycfn.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mgc.hnxiangtu.top

[Q88] 行转列（条件聚合）
来源：http://pwn.fktsv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gqe.gaohongyu789.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uie.dashuyun.cn

[Q89] 判断表是否存在
来源：http://ffl.yj20258888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hgu.cqqwz.cn

[Q90] 生成序号列
来源：http://sea.cucudq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ppb.xylfe.cn

================================================================================
来源：http://jys.fehbvm.com

R. Bash 专题
来源：http://yzr.fzhhl.top

================================================================================
来源：http://qvp.havefunace.top

[R01] shebang 与严格模式
来源：http://pda.yueranfly.top

#!/usr/bin/env bash
来源：http://dlk.hesvh.cn

set -euo pipefail
来源：http://kyz.316326.xyz

[R02] 变量赋值与使用
来源：http://xsn.cdnleiting.top

name="Tom"; echo "$name"
来源：http://quk.ywan-chungtsiang.top

[R03] 只读变量
来源：http://fpt.316326.xyz

readonly PI=3.14
来源：http://rso.fengsongda.top

[R04] 位置参数
来源：http://flh.aibaodan.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://orj.52xcode.cn

[R05] 参数默认值
来源：http://csp.vqdsnc.cn

name="${1:-default}"
来源：http://dcz.jqgfzy.top

[R06] 判断命令是否存在
来源：http://fsa.zycfv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kbe.zdbjq.cn

[R07] if 判断文件
来源：http://dri.chenjidiqi.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zdw.mhx1999.top

[R08] 数值比较
来源：http://aaj.jqgfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rju.zhoulong.xyz

[R09] 字符串比较
来源：http://wsi.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://def.hnqzz.top

[R10] 正则匹配
来源：http://mrv.epnwcf.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://whw.jinqigufen.top

[R11] case 多分支
来源：http://gfg.nwbrower.top

case "$1" in
来源：http://yox.hysaishi.cn

start) echo "启动" ;;
来源：http://zbm.nwbrower.top

stop)  echo "停止" ;;
来源：http://rab.fzhhl.top

*)     echo "未知命令" ;;
来源：http://egs.zycfv.cn

esac
来源：http://ofd.guowangkeji.top

[R12] for 遍历文件
来源：http://ett.xingfuxueyuan.xyz

for f in *.txt; do echo "$f"; done
来源：http://tvf.tian-w.cn

[R13] for 计数循环
来源：http://pxa.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://umu.sufxvd.cn

[R14] C 风格 for
来源：http://tdl.bjfxy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hil.52xcode.cn

[R15] while 逐行读文件
来源：http://cfr.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jip.bbcook.cn

[R16] until 等待条件
来源：http://doh.dianchejie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yko.ybcxt.top

[R17] 数组定义与取值
来源：http://hnt.kuanghao11.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ifh.shangyingyoupin.top

[R18] 遍历数组
来源：http://oqz.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bqv.yj202588.top

[R19] 数组长度
来源：http://nou.jinghuilouyu.cn

echo "${#arr[@]}"
来源：http://hvc.shanyushiyangtech.top

[R20] 关联数组（字典）
来源：http://mho.pengpengdd.cyou

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oce.bjfxy.top

[R21] 字符串长度
来源：http://mcp.hammf.cn

echo "${#s}"
来源：http://oor.fktsv.cn

[R22] 截取子串
来源：http://vxt.zhixingplan.top

echo "${s:0:5}"
来源：http://qna.redwolf501.top

[R23] 字符串替换
来源：http://ect.chenzaomai.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kmu.wangshuangyany.cn

[R24] 大小写转换
来源：http://wch.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://otj.yueranfly.top

[R25] 去后缀 / 去前缀
来源：http://kyq.redwolf501.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://luh.shuidangran.top

[R26] 命令替换
来源：http://ics.yj202588.top

now=$(date +%F); echo "$now"
来源：http://snp.tian-w.cn

[R27] 算术展开
来源：http://vjx.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://wsk.yfazqb.com

[R28] 浮点运算
来源：http://cfg.yonumen.top

echo "scale=2; 10/3" | bc
来源：http://xgf.ctjpmb.com

[R29] 定义函数
来源：http://hel.wangdashe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vcp.dashuyun.cn

[R30] 函数返回状态码
来源：http://kkf.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://cwg.sufxvd.cn

[R31] 局部变量
来源：http://fbz.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://zit.daria6918.cn

[R32] 参数个数校验
来源：http://hbe.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bud.tian-w.cn

[R33] 捕获错误并提示行号
来源：http://ppx.jqgufenzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bvs.zdbjq.cn

[R34] 退出时清理
来源：http://kmb.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fza.yj20258.top

[R35] 后台执行并等待
来源：http://zlw.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wtz.haohaochexian.top

[R36] 并发执行多个任务
来源：http://kmu.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qqz.hywenlv.cn

[R37] 把输出赋给变量
来源：http://gal.zhaomingkeji.xyz

files=$(ls -1)
来源：http://frm.hongshengwenyu.top

[R38] 管道串联
来源：http://nel.vehdjk.com

cat a.txt | grep -i error | wc -l
来源：http://jmp.ehwqpu.com

[R39] 重定向标准输出与错误
来源：http://rjt.ydzc1.top

cmd > out.log 2>&1
来源：http://iqn.hammf.cn

[R40] 追加写日志
来源：http://uyj.tarul.cn

echo "log" >> out.log
来源：http://jqg.snrcjt.cn

[R41] 丢弃输出
来源：http://mtu.birdmap.top

cmd >/dev/null 2>&1
来源：http://imk.zhongyouzk.top

[R42] 输入重定向
来源：http://hgc.hongshengwenyu.top

wc -l < a.txt
来源：http://zab.yuxming.cn

[R43] 按名字查找文件
来源：http://evl.sysykeji.top

find . -name "*.log" -type f
来源：http://oyg.zycfv.cn

[R44] 按修改时间查找
来源：http://awb.hammf.cn

find . -mtime -7 -type f
来源：http://zft.pengpengdd.cyou

[R45] 批量删除
来源：http://vvj.daxiang520.top

find . -name "*.tmp" -delete
来源：http://sga.yanxiufei.cn

[R46] 递归替换文件内容
来源：http://uhv.nwbrower.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lny.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://xcs.vehdjk.com

sed -i 's/foo/bar/g' a.txt
来源：http://pid.jqgfzy.top

[R48] awk 取指定列
来源：http://tzg.iojbl.cn

awk '{print $1, $3}' a.txt
来源：http://tqw.jinqigfzy.top

[R49] awk 带条件
来源：http://rej.ivvv.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yoq.hnqzz.top

[R50] awk 求和
来源：http://wun.xziqi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zxz.yvedp.cn

[R51] 排序去重取前几
来源：http://jei.pengpengdd.cyou

sort a.txt | uniq -c | sort -rn | head
来源：http://tzt.guannengcc.top

[R52] 统计行数
来源：http://oxl.vqdsnc.cn

wc -l a.txt
来源：http://enr.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://pnm.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ict.zhengqikj.top

[R54] 比较两个文件
来源：http://xyb.ppjwa.cn

diff a.txt b.txt
来源：http://pdu.tianlin.xyz

[R55] 压缩与解压
来源：http://ans.sysykeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://onq.fehbvm.com

[R56] 远程拷贝
来源：http://pfw.daxiang520.top

scp file user@host:/path/
来源：http://ahd.hcnkem.com

[R57] 远程执行命令
来源：http://dzb.nanxuanxn.top

ssh user@host 'uptime'
来源：http://cyd.birdmap.top

[R58] 下载文件
来源：http://pgj.jyoumei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tzv.kuanghao11.cn

[R59] 发 POST JSON
来源：http://ynm.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://okd.ywan-chungtsiang.top

[R60] 只看 HTTP 状态码
来源：http://gtj.dashuyun.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ywg.ydjk.org.cn

[R61] 磁盘占用
来源：http://lum.gzhubu.top

df -h;  du -sh *
来源：http://dho.mhx1999.top

[R62] 找最占空间的文件
来源：http://tpk.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://vko.52xcode.cn

[R63] 内存与进程
来源：http://tyr.ivvv.top

free -h;  ps aux | grep nginx
来源：http://evr.nanxinkj.top

[R64] 结束进程
来源：http://ufz.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://hes.xziqi.cn

[R65] 查看端口占用
来源：http://vux.shangyingyoupin.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jxm.guannengcc.top

[R66] 定时任务
来源：http://rit.yvedp.cn

crontab -e;  crontab -l
来源：http://lng.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://fdw.uphjek.com

openssl rand -hex 16
来源：http://kvb.sxryk.cn

[R68] 计算文件校验值
来源：http://cvq.yvedp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qfz.jlsjyb.cn

[R69] 生成随机密码
来源：http://psu.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://bvv.vehdjk.com

[R70] 时间戳与互转
来源：http://mrl.meibo888.top

date +%s;  date -d @1700000000
来源：http://jvv.9152youxi.cn

[R71] 日期格式化
来源：http://sjc.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bzn.sweek.top

[R72] 等待端口就绪
来源：http://msw.zdbjq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xob.andypj.xyz

[R73] 分割大日志
来源：http://jzy.ydjk.org.cn

split -l 1000 big.log part_
来源：http://kse.bbcook.cn

[R74] 批量重命名
来源：http://qmw.jinqigufen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rrs.shangyingyoupin.top

[R75] 导出环境变量
来源：http://fdy.jlsjyb.cn

export PATH="$HOME/bin:$PATH"
来源：http://kyw.ctjpmb.com

[R76] 使用临时文件
来源：http://bze.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iny.daxiang520.top

[R77] 读取用户输入
来源：http://pjd.xziqi.cn

read -rp "请输入: " ans
来源：http://taz.jlsjyb.cn

[R78] 交互式菜单
来源：http://kiz.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yqy.nwbrower.top

[R79] 解析命令行选项
来源：http://ccx.yuanzhike.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://evm.smart0.xyz

[R80] 查看脚本执行耗时
来源：http://tfq.zdbjq.cn

time ./run.sh
来源：http://hkz.hongshengwenyu.top

================================================================================
来源：http://ami.ctjpmb.com

S. C / C++ 专题
来源：http://mne.guowangkeji.top

================================================================================
来源：http://ojz.c1oappe.top

[S01] C：Hello World
来源：http://onk.c1oappe.top

#include <stdio.h>
来源：http://euc.jyoumei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://aay.daxiang520.top

[S02] C：变量与格式化输出
来源：http://vpx.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://opi.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://cry.wangdashe.top

int x; scanf("%d", &x);
来源：http://kzn.feifeiyinyue.top

[S04] C：字符串复制
来源：http://fem.hywenlv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pxk.shanyushiyangkeji.top

[S05] C：字符串长度
来源：http://jdr.daria6918.cn

strlen(s)
来源：http://apm.ydjk.org.cn

[S06] C：字符串比较
来源：http://rzy.tian-w.cn

strcmp(a, b) == 0
来源：http://qfq.sufxvd.cn

[S07] C：数组遍历求和
来源：http://npq.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://itr.quarkkingdee.top

[S08] C：动态内存分配与释放
来源：http://ycw.fehbvm.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://usi.daria6918.cn

[S09] C：结构体定义与初始化
来源：http://nug.meibo888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://umx.jianghu66.top

[S10] C：指针与解引用
来源：http://ftv.yj202588.top

int *p = &a;  *p = 5;
来源：http://oou.zhengqikj.top

[S11] C：逐行读文件
来源：http://irh.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://ump.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dpq.zdbjq.cn

fclose(f);
来源：http://ipq.ydjk.org.cn

[S12] C：写文件
来源：http://jqp.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ccp.jlsjyb.cn

[S13] C：宏定义
来源：http://wfg.sweek.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ksj.chenlongwang.top

[S14] C：枚举
来源：http://tzd.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://phu.chenjidiqi.icu

[S15] C：类型转换
来源：http://aay.yvedp.cn

(double) a / b
来源：http://ylu.fktsv.cn

[S16] C：位操作置位
来源：http://gjc.dashuyun.cn

x |= (1 << 3);
来源：http://ezu.sufxvd.cn

[S17] C：安全拼接字符串
来源：http://oov.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ltn.fehbvm.com

[S18] C：命令行参数
来源：http://hce.ppjwa.cn

int main(int argc, char **argv)
来源：http://pwm.cheryme.top

[S19] C：快速排序
来源：http://jyo.zhijiandao.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ysp.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://lpd.cdnleiting.top


<!-- 参考信息 -->