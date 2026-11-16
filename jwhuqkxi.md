代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tlj.yj20258888.top

[Q50] 批量更新
来源：http://dce.yueranfly.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gvw.feifeiyinyue.top

[Q51] 用子查询更新
来源：http://htp.ydzc1.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zte.cashguo.top

[Q52] 删除指定行
来源：http://xzh.bbcook.cn

DELETE FROM users WHERE id = 10;
来源：http://hdt.xinyue.icu

[Q53] 按条件删除
来源：http://mdg.dianchejie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iri.chenjidiqi.icu

[Q54] 清空表
来源：http://elm.xylfe.cn

TRUNCATE TABLE logs;
来源：http://scp.zhaomingkeji.xyz

[Q55] 排名（并列占位）
来源：http://onx.daxiang520.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://evs.jinghuilouyu.cn

[Q56] 密集排名（并列不占位）
来源：http://znb.ivvv.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sqg.jinghuilouyu.cn

[Q57] 行号
来源：http://gba.cqqwz.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vkp.nwbrower.top

[Q58] 累计求和
来源：http://ifm.yj202588.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ird.wangshuangyany.cn

[Q59] 分组内累计
来源：http://xnn.fanxiaobao.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jmi.ywan-chungtsiang.top

[Q60] 取上一行 / 下一行
来源：http://qzf.hywenlv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pvg.pengpengdd.cyou

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://drn.tian-w.cn

[Q61] 移动平均
来源：http://jge.daria6918.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ijy.sweek.top

[Q62] 分组占比
来源：http://prt.xinyue.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wlw.9152youxi.cn

[Q63] 开启事务
来源：http://msy.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sni.chenzaomai.com

[Q64] 提交事务
来源：http://zqa.xuanzx.com

COMMIT;
来源：http://xgh.sweek.top

[Q65] 回滚事务
来源：http://psx.sysykeji.top

ROLLBACK;
来源：http://jui.gzhubu.top

[Q66] 行锁查询
来源：http://lwb.jlsjyb.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hug.hongshengwenyu.top

[Q67] 设置隔离级别
来源：http://wfi.jinyuanbaomall.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xsl.meibo888.top

[Q68] 保存点
来源：http://dyf.yonumen.top

SAVEPOINT sp1;
来源：http://weu.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://vxu.zhixingplan.top

[Q69] 查看执行计划
来源：http://tic.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xyb.zhoulong.xyz

[Q70] 更新统计信息
来源：http://aii.fehbvm.com

ANALYZE TABLE users;
来源：http://vuk.hnxiangtu.top

[Q71] 查看建表语句
来源：http://big.hfpthk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qky.birdmap.top

[Q72] 查看索引
来源：http://nxy.xylfe.cn

SHOW INDEX FROM users;
来源：http://foh.daxiang520.top

[Q73] 查看表状态
来源：http://zfj.andypj.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://voy.sysykeji.top

[Q74] 强制使用索引
来源：http://hkk.chenzaomai.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lsz.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://clr.yanxiufei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://thq.xinyue.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://css.daria6918.cn

[Q76] 按天统计
来源：http://uwy.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qqd.tian-w.cn

[Q77] 时间加减
来源：http://khl.daria6918.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xqr.xingfuxueyuan.xyz

[Q78] 当前时间
来源：http://buh.52xcode.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qgm.uphjek.com

[Q79] 字符串拼接
来源：http://wvx.yuxming.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zyz.ehwqpu.com

[Q80] 字符串截取
来源：http://hwg.yfazqb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iyh.yj202588.top

[Q81] 字符串替换
来源：http://fjm.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pld.cdnleiting.top

[Q82] 字符长度与字节长度
来源：http://hym.haohaochexian.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rdl.9152youxi.cn

[Q83] 大小写转换
来源：http://rrf.hywenlv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nto.smart0.xyz

[Q84] 去除首尾空格
来源：http://seu.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://uij.ehwqpu.com

[Q85] 数值取整
来源：http://vpk.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nop.epnwcf.com

[Q86] 读取 JSON 字段
来源：http://kym.smart0.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nch.sweek.top

[Q87] JSON 字段做条件
来源：http://pql.hnxiangtu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dwk.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://whg.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://shk.zhiwuduotai.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://say.chenjidiqi.icu

[Q89] 判断表是否存在
来源：http://mer.yj20258888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qct.sxryk.cn

[Q90] 生成序号列
来源：http://chj.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aei.gaohongyu789.top

================================================================================
来源：http://piz.meibo888.top

R. Bash 专题
来源：http://bjd.yangfankeji.com

================================================================================
来源：http://zlm.redwolf501.top

[R01] shebang 与严格模式
来源：http://ddq.cucudq.cn

#!/usr/bin/env bash
来源：http://kcw.vqdsnc.cn

set -euo pipefail
来源：http://qjq.uphjek.com

[R02] 变量赋值与使用
来源：http://tlq.yuanzhike.top

name="Tom"; echo "$name"
来源：http://zup.xylfe.cn

[R03] 只读变量
来源：http://rcl.hysaishi.cn

readonly PI=3.14
来源：http://lph.shanyushiyangkeji.top

[R04] 位置参数
来源：http://zgs.yanxiufei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rmq.hesvh.cn

[R05] 参数默认值
来源：http://dpj.zhongyouzk.top

name="${1:-default}"
来源：http://nlb.ppjwa.cn

[R06] 判断命令是否存在
来源：http://xso.ppjwa.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iji.nwbrower.top

[R07] if 判断文件
来源：http://bzy.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zfg.xziqi.cn

[R08] 数值比较
来源：http://feb.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jct.pengpengdd.cyou

[R09] 字符串比较
来源：http://peq.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vhl.yj20258.top

[R10] 正则匹配
来源：http://ksp.daria6918.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mll.ehwqpu.com

[R11] case 多分支
来源：http://gcx.shanyushiyangtech.top

case "$1" in
来源：http://bix.jlsjyb.cn

start) echo "启动" ;;
来源：http://xed.ywan-chungtsiang.top

stop)  echo "停止" ;;
来源：http://kip.gotoacloud.top

*)     echo "未知命令" ;;
来源：http://zwq.sysykeji.top

esac
来源：http://zbd.uphjek.com

[R12] for 遍历文件
来源：http://cvg.pengpengdd.cyou

for f in *.txt; do echo "$f"; done
来源：http://vmy.c1oappe.top

[R13] for 计数循环
来源：http://thb.guannengcc.top

for i in {1..10}; do echo "$i"; done
来源：http://icc.zhengqikj.top

[R14] C 风格 for
来源：http://wuf.gzhubu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kyi.vqdsnc.cn

[R15] while 逐行读文件
来源：http://nxj.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ppg.uphjek.com

[R16] until 等待条件
来源：http://zoh.gotoacloud.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mzd.shzxlz.cn

[R17] 数组定义与取值
来源：http://fhf.cucudq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hkr.redwolf501.top

[R18] 遍历数组
来源：http://qqn.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mic.guannengcc.top

[R19] 数组长度
来源：http://hji.jqgfzy.top

echo "${#arr[@]}"
来源：http://lqy.fzhhl.top

[R20] 关联数组（字典）
来源：http://yxz.hysaishi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rde.ydzc1.top

[R21] 字符串长度
来源：http://ynn.chenlongwang.top

echo "${#s}"
来源：http://ofr.bjfxy.top

[R22] 截取子串
来源：http://xus.birdmap.top

echo "${s:0:5}"
来源：http://dwt.tarul.cn

[R23] 字符串替换
来源：http://flq.cashguo.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://plk.tianlin.xyz

[R24] 大小写转换
来源：http://ymw.shuidangran.top

echo "${s^^}"; echo "${s,,}"
来源：http://ewg.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://kgj.cashguo.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lbn.yongpay.top

[R26] 命令替换
来源：http://qug.xuetiantiany.cn

now=$(date +%F); echo "$now"
来源：http://lbl.sufxvd.cn

[R27] 算术展开
来源：http://wxu.hcnkem.com

echo $((1 + 2 * 3))
来源：http://zlp.mhx1999.top

[R28] 浮点运算
来源：http://pyh.ywan-chungtsiang.top

echo "scale=2; 10/3" | bc
来源：http://zoj.gzhubu.top

[R29] 定义函数
来源：http://htt.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jrv.hnxiangtu.top

[R30] 函数返回状态码
来源：http://bnc.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://ifi.vehdjk.com

[R31] 局部变量
来源：http://ihp.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://lwz.yuanzhike.top

[R32] 参数个数校验
来源：http://iys.fzhhl.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ntd.zhengqikj.top

[R33] 捕获错误并提示行号
来源：http://lyw.zhengqikj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zew.aibaodan.cn

[R34] 退出时清理
来源：http://nkt.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://yiz.jqgufenzy.top

[R35] 后台执行并等待
来源：http://jjm.vehdjk.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ehs.xinyue.icu

[R36] 并发执行多个任务
来源：http://jvx.52xcode.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gfg.ehwqpu.com

[R37] 把输出赋给变量
来源：http://zzy.cdnleiting.top

files=$(ls -1)
来源：http://xym.zhaomingkeji.xyz

[R38] 管道串联
来源：http://itf.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://ytn.chenzaomai.com

[R39] 重定向标准输出与错误
来源：http://rdt.tian-w.cn

cmd > out.log 2>&1
来源：http://oym.dianchejie.cn

[R40] 追加写日志
来源：http://den.fanxiaobao.xyz

echo "log" >> out.log
来源：http://vfa.316326.xyz

[R41] 丢弃输出
来源：http://poo.svipenyu.cn

cmd >/dev/null 2>&1
来源：http://vfk.0kj1m.cn

[R42] 输入重定向
来源：http://ivr.cheryme.top

wc -l < a.txt
来源：http://rhn.hcnkem.com

[R43] 按名字查找文件
来源：http://vwj.yanxiufei.cn

find . -name "*.log" -type f
来源：http://fmk.daxiang520.top

[R44] 按修改时间查找
来源：http://lpu.pycfn.com

find . -mtime -7 -type f
来源：http://ezw.nanxinkj.top

[R45] 批量删除
来源：http://eas.zdbjq.cn

find . -name "*.tmp" -delete
来源：http://vkj.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://dyi.jlsjyb.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ryt.hesvh.cn

[R47] sed 单行替换
来源：http://jdz.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://syf.wangshuangyany.cn

[R48] awk 取指定列
来源：http://oxg.hongshengwenyu.top

awk '{print $1, $3}' a.txt
来源：http://mqy.meibo888.top

[R49] awk 带条件
来源：http://dvc.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dkh.pengpengdd.cyou

[R50] awk 求和
来源：http://gqp.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fno.pycfn.com

[R51] 排序去重取前几
来源：http://pce.yj20258.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rqr.ppjwa.cn

[R52] 统计行数
来源：http://tkl.iojbl.cn

wc -l a.txt
来源：http://lni.yanxiufei.cn

[R53] 查看文件头与实时尾
来源：http://wts.xuetiantiany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ujh.jianghu66.top

[R54] 比较两个文件
来源：http://ycu.hammf.cn

diff a.txt b.txt
来源：http://aik.zhiwuduotai.top

[R55] 压缩与解压
来源：http://fsf.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iwf.iojbl.cn

[R56] 远程拷贝
来源：http://zyg.fengsongda.top

scp file user@host:/path/
来源：http://okc.aibaodan.cn

[R57] 远程执行命令
来源：http://rap.sxryk.cn

ssh user@host 'uptime'
来源：http://fay.yj202588.top

[R58] 下载文件
来源：http://shf.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jwk.316326.xyz

[R59] 发 POST JSON
来源：http://qkb.redwolf501.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://aiy.fehbvm.com

[R60] 只看 HTTP 状态码
来源：http://nni.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://myc.zhiwuduotai.top

[R61] 磁盘占用
来源：http://kxi.bjfxy.top

df -h;  du -sh *
来源：http://cgx.c1oappe.top

[R62] 找最占空间的文件
来源：http://eoq.yonumen.top

du -ah . | sort -rh | head -10
来源：http://ica.zhaomingkeji.xyz

[R63] 内存与进程
来源：http://hhb.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://rem.guannengcc.top

[R64] 结束进程
来源：http://eke.zhiwuduotai.top

kill -9 $(pgrep -f app.py)
来源：http://zvz.snrcjt.cn

[R65] 查看端口占用
来源：http://cex.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rwu.sysykeji.top

[R66] 定时任务
来源：http://wor.nwbrower.top

crontab -e;  crontab -l
来源：http://jli.hysaishi.cn

[R67] 生成随机十六进制串
来源：http://yfz.zhoulong.xyz

openssl rand -hex 16
来源：http://hit.cashguo.top

[R68] 计算文件校验值
来源：http://wcg.cdnleiting.top

sha256sum a.txt;  md5sum a.txt
来源：http://oaw.fehbvm.com

[R69] 生成随机密码
来源：http://mfu.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://wpi.hysaishi.cn

[R70] 时间戳与互转
来源：http://zbw.dianchejie.cn

date +%s;  date -d @1700000000
来源：http://irn.316326.xyz

[R71] 日期格式化
来源：http://xmy.epnwcf.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://thq.svipenyu.cn

[R72] 等待端口就绪
来源：http://lht.chenzaomai.com

until nc -z localhost 3306; do sleep 1; done
来源：http://xld.zhengqikj.top

[R73] 分割大日志
来源：http://akr.smart0.xyz

split -l 1000 big.log part_
来源：http://ppc.jinqigufen.top

[R74] 批量重命名
来源：http://agh.sxryk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fys.tianlin.xyz

[R75] 导出环境变量
来源：http://hjt.zhixingplan.top

export PATH="$HOME/bin:$PATH"
来源：http://kln.hnqzz.top

[R76] 使用临时文件
来源：http://jfa.ehwqpu.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vyq.pengpengdd.cyou

[R77] 读取用户输入
来源：http://ynq.jlsjyb.cn

read -rp "请输入: " ans
来源：http://boa.sweek.top

[R78] 交互式菜单
来源：http://zce.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://szv.shanyushiyangkeji.top

[R79] 解析命令行选项
来源：http://qzi.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yrn.yvedp.cn

[R80] 查看脚本执行耗时
来源：http://mtx.wangdashe.top

time ./run.sh
来源：http://acw.yonumen.top

================================================================================
来源：http://gou.ctjpmb.com

S. C / C++ 专题
来源：http://ebt.daxiang520.top

================================================================================
来源：http://jwl.zhijiandao.cn

[S01] C：Hello World
来源：http://jcq.yangfankeji.com

#include <stdio.h>
来源：http://cwi.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tjo.tianlin.xyz

[S02] C：变量与格式化输出
来源：http://ojb.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://zkt.shuidangran.top

[S03] C：读入整数
来源：http://sav.yj202588.top

int x; scanf("%d", &x);
来源：http://xvc.bjfxy.top

[S04] C：字符串复制
来源：http://gzo.jqgfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://mkx.xylfe.cn

[S05] C：字符串长度
来源：http://plc.jinyuanbaomall.cn

strlen(s)
来源：http://shd.yj20258.top

[S06] C：字符串比较
来源：http://ggf.guannengcc.top

strcmp(a, b) == 0
来源：http://izv.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://kur.chenjidiqi.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jza.0kj1m.cn

[S08] C：动态内存分配与释放
来源：http://gvm.fengsongda.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lng.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://vac.hesvh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lyx.daria6918.cn

[S10] C：指针与解引用
来源：http://kye.redwolf501.top

int *p = &a;  *p = 5;
来源：http://ktr.bbcook.cn

[S11] C：逐行读文件
来源：http://cwu.snrcjt.cn

FILE *f = fopen("a.txt", "r");
来源：http://fye.52xcode.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://spd.yueranfly.top

fclose(f);
来源：http://pvz.fanxiaobao.xyz

[S12] C：写文件
来源：http://sja.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qjq.tarul.cn

[S13] C：宏定义
来源：http://cjd.ppjwa.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pbw.snrcjt.cn

[S14] C：枚举
来源：http://kyk.pycfn.com

enum Color { RED, GREEN, BLUE };
来源：http://fjc.shanyushiyangtech.top

[S15] C：类型转换
来源：http://tbg.jinqigfzy.top

(double) a / b
来源：http://hup.feifeiyinyue.top

[S16] C：位操作置位
来源：http://zny.0kj1m.cn

x |= (1 << 3);
来源：http://xaf.sxryk.cn

[S17] C：安全拼接字符串
来源：http://yob.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://smv.jlsjyb.cn

[S18] C：命令行参数
来源：http://snb.gzhubu.top

int main(int argc, char **argv)
来源：http://imq.jlsjyb.cn

[S19] C：快速排序
来源：http://elw.snrcjt.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yag.tianlin.xyz

[S20] C：二分查找
来源：http://ebi.pycfn.com


<!-- 参考信息 -->