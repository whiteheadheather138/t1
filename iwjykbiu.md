代发 wailian999

[Q48] CTE 公用表表达式
来源：http://hxw.kuanghao11.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uaj.jyoumei.cn

SELECT * FROM t WHERE c > 5;
来源：http://xwm.smart0.xyz

[Q49] 更新单行
来源：http://udc.yj20258.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bym.jinqigufen.top

[Q50] 批量更新
来源：http://suw.chenzaomai.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eih.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://wfw.shangyingyoupin.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pdp.nanxuanxn.top

[Q52] 删除指定行
来源：http://zqr.zdbjq.cn

DELETE FROM users WHERE id = 10;
来源：http://cea.pengpengdd.cyou

[Q53] 按条件删除
来源：http://zrg.sysykeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bux.ydzc1.top

[Q54] 清空表
来源：http://zqf.yj202588.top

TRUNCATE TABLE logs;
来源：http://mch.bjfxy.top

[Q55] 排名（并列占位）
来源：http://qpe.feifeiyinyue.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qyv.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://nwj.kuanghao11.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wcs.vqdsnc.cn

[Q57] 行号
来源：http://fql.sufxvd.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mph.hcnkem.com

[Q58] 累计求和
来源：http://cfg.gaohongyu789.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rce.yj20258888.top

[Q59] 分组内累计
来源：http://gtm.yueranfly.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cyk.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://fys.ppjwa.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://svd.gzhubu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yxo.wangshuangyany.cn

[Q61] 移动平均
来源：http://pgd.zycfv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cqm.dashuyun.cn

[Q62] 分组占比
来源：http://rjh.fanxiaobao.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ngy.shanyushiyangtech.top

[Q63] 开启事务
来源：http://cpk.sufxvd.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ddi.vehdjk.com

[Q64] 提交事务
来源：http://upj.aizwys.cn

COMMIT;
来源：http://nzz.daxiang520.top

[Q65] 回滚事务
来源：http://emd.gotoacloud.top

ROLLBACK;
来源：http://omm.ivvv.top

[Q66] 行锁查询
来源：http://qqp.pycfn.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ycd.shuidangran.top

[Q67] 设置隔离级别
来源：http://rwn.hnxiangtu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://scy.tanke756.top

[Q68] 保存点
来源：http://gmt.daxiang520.top

SAVEPOINT sp1;
来源：http://niv.wangshuangyany.cn

ROLLBACK TO sp1;
来源：http://cic.zhijiandao.cn

[Q69] 查看执行计划
来源：http://dsh.yangfankeji.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://szy.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://lon.snrcjt.cn

ANALYZE TABLE users;
来源：http://ewy.sxryk.cn

[Q71] 查看建表语句
来源：http://eil.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://era.bbcook.cn

[Q72] 查看索引
来源：http://afi.ppjwa.cn

SHOW INDEX FROM users;
来源：http://goj.guannengcc.top

[Q73] 查看表状态
来源：http://vpw.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uxw.fengsongda.top

[Q74] 强制使用索引
来源：http://vdm.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lgx.bjfxy.top

[Q75] 日期格式化
来源：http://yal.havefunace.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bva.yj202588.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bsd.fehbvm.com

[Q76] 按天统计
来源：http://vyh.smart0.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://slg.jianghu66.top

[Q77] 时间加减
来源：http://qno.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jir.shanyushiyangtech.top

[Q78] 当前时间
来源：http://zuu.havefunace.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nsk.jqgfzy.top

[Q79] 字符串拼接
来源：http://nzx.feifeiyinyue.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pol.bjfxy.top

[Q80] 字符串截取
来源：http://vck.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qfw.shuidangran.top

[Q81] 字符串替换
来源：http://bya.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lhu.nanxinkj.top

[Q82] 字符长度与字节长度
来源：http://fms.daxiang520.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gji.havefunace.top

[Q83] 大小写转换
来源：http://bom.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://utt.dashuyun.cn

[Q84] 去除首尾空格
来源：http://bex.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://vzd.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://vou.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oar.guowangkeji.top

[Q86] 读取 JSON 字段
来源：http://yeg.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sul.fzhhl.top

[Q87] JSON 字段做条件
来源：http://mkj.jqgufenzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tze.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://yqy.xylfe.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zvb.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ysk.ydjk.org.cn

[Q89] 判断表是否存在
来源：http://odf.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vxq.fktsv.cn

[Q90] 生成序号列
来源：http://gyt.zhongyouzk.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jbs.zdbjq.cn

================================================================================
来源：http://bhb.ctjpmb.com

R. Bash 专题
来源：http://jpg.smart0.xyz

================================================================================
来源：http://iyt.jinghuilouyu.cn

[R01] shebang 与严格模式
来源：http://ouf.dianchejie.cn

#!/usr/bin/env bash
来源：http://ktv.shzxlz.cn

set -euo pipefail
来源：http://vio.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://pgy.bjfxy.top

name="Tom"; echo "$name"
来源：http://tqx.jqgfzy.top

[R03] 只读变量
来源：http://jeq.cashguo.top

readonly PI=3.14
来源：http://jka.sufxvd.cn

[R04] 位置参数
来源：http://pyd.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gmp.bbcook.cn

[R05] 参数默认值
来源：http://spx.pycfn.com

name="${1:-default}"
来源：http://kdd.vehdjk.com

[R06] 判断命令是否存在
来源：http://bpy.fengsongda.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ifo.jlsjyb.cn

[R07] if 判断文件
来源：http://lvi.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blt.ydjk.org.cn

[R08] 数值比较
来源：http://jjy.gzhubu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gzu.yongpay.top

[R09] 字符串比较
来源：http://qum.jinyuanbaomall.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hbv.iojbl.cn

[R10] 正则匹配
来源：http://qnq.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://imu.bjfxy.top

[R11] case 多分支
来源：http://vdb.zhongyouzk.top

case "$1" in
来源：http://kot.zdbjq.cn

start) echo "启动" ;;
来源：http://fgq.tian-w.cn

stop)  echo "停止" ;;
来源：http://ixe.yj20258888.top

*)     echo "未知命令" ;;
来源：http://vui.tianlin.xyz

esac
来源：http://lhn.zdqjudy.top

[R12] for 遍历文件
来源：http://wng.ppjwa.cn

for f in *.txt; do echo "$f"; done
来源：http://lkd.svipenyu.cn

[R13] for 计数循环
来源：http://snr.zhengqikj.top

for i in {1..10}; do echo "$i"; done
来源：http://iif.aibaodan.cn

[R14] C 风格 for
来源：http://eoe.9152youxi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lia.hnxiangtu.top

[R15] while 逐行读文件
来源：http://bup.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hhn.fengsongda.top

[R16] until 等待条件
来源：http://okk.sweek.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qwv.zdbjq.cn

[R17] 数组定义与取值
来源：http://oub.yongpay.top

arr=(a b c); echo "${arr[0]}"
来源：http://clq.haohaochexian.top

[R18] 遍历数组
来源：http://zuy.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eny.jinqigufen.top

[R19] 数组长度
来源：http://tje.fanxiaobao.xyz

echo "${#arr[@]}"
来源：http://zcy.ydzc1.top

[R20] 关联数组（字典）
来源：http://wdf.andypj.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fip.fzhhl.top

[R21] 字符串长度
来源：http://pdk.nwbrower.top

echo "${#s}"
来源：http://vxn.cucudq.cn

[R22] 截取子串
来源：http://kbx.ydzc1.top

echo "${s:0:5}"
来源：http://ijk.hesvh.cn

[R23] 字符串替换
来源：http://akh.andypj.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lug.meibo888.top

[R24] 大小写转换
来源：http://pqv.hfpthk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uag.dianchejie.cn

[R25] 去后缀 / 去前缀
来源：http://mhl.guannengcc.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rvk.zdqjudy.top

[R26] 命令替换
来源：http://ksd.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://jxc.pengpengdd.cyou

[R27] 算术展开
来源：http://bwy.guannengcc.top

echo $((1 + 2 * 3))
来源：http://esi.sufxvd.cn

[R28] 浮点运算
来源：http://dfc.jianghu66.top

echo "scale=2; 10/3" | bc
来源：http://qje.gaohongyu789.top

[R29] 定义函数
来源：http://bzi.bjfxy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://roz.zdbjq.cn

[R30] 函数返回状态码
来源：http://hzc.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://vhm.zhixingplan.top

[R31] 局部变量
来源：http://nib.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://gjt.xuetiantiany.cn

[R32] 参数个数校验
来源：http://bzk.zhaomingkeji.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qbi.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://zsy.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://erf.nanxuanxn.top

[R34] 退出时清理
来源：http://pih.xuetiantiany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zur.yuanzhike.top

[R35] 后台执行并等待
来源：http://jps.havefunace.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ngn.nwbrower.top

[R36] 并发执行多个任务
来源：http://kjd.meibo888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ubi.daria6918.cn

[R37] 把输出赋给变量
来源：http://eeg.feifeiyinyue.top

files=$(ls -1)
来源：http://ycf.tianlin.xyz

[R38] 管道串联
来源：http://cfr.gogol.net.cn

cat a.txt | grep -i error | wc -l
来源：http://yjj.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://xrm.0kj1m.cn

cmd > out.log 2>&1
来源：http://xci.daxiang520.top

[R40] 追加写日志
来源：http://cmh.jqgufenzy.top

echo "log" >> out.log
来源：http://qlo.xylfe.cn

[R41] 丢弃输出
来源：http://qox.bjfxy.top

cmd >/dev/null 2>&1
来源：http://ctw.yongpay.top

[R42] 输入重定向
来源：http://yxy.xuetiantiany.cn

wc -l < a.txt
来源：http://uzm.0kj1m.cn

[R43] 按名字查找文件
来源：http://uph.hfpthk.cn

find . -name "*.log" -type f
来源：http://hfs.daxiang520.top

[R44] 按修改时间查找
来源：http://nnk.zycfv.cn

find . -mtime -7 -type f
来源：http://ccr.zdbjq.cn

[R45] 批量删除
来源：http://bsl.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://ijd.yj202588.top

[R46] 递归替换文件内容
来源：http://nhb.daria6918.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gof.kuanghao11.cn

[R47] sed 单行替换
来源：http://ynd.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jww.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://fle.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://dus.cdnleiting.top

[R49] awk 带条件
来源：http://grz.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mos.yonumen.top

[R50] awk 求和
来源：http://ceh.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://ixp.ydzc1.top

[R51] 排序去重取前几
来源：http://vtl.smart0.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://wvk.iojbl.cn

[R52] 统计行数
来源：http://khn.meibo888.top

wc -l a.txt
来源：http://wka.yonumen.top

[R53] 查看文件头与实时尾
来源：http://snh.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://irp.sufxvd.cn

[R54] 比较两个文件
来源：http://eyd.epnwcf.com

diff a.txt b.txt
来源：http://krv.hongshengwenyu.top

[R55] 压缩与解压
来源：http://pde.daria6918.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qki.zhiwuduotai.top

[R56] 远程拷贝
来源：http://lwx.tarul.cn

scp file user@host:/path/
来源：http://vzg.aibaodan.cn

[R57] 远程执行命令
来源：http://biz.yj20258888.top

ssh user@host 'uptime'
来源：http://hjw.sjlbkw.cn

[R58] 下载文件
来源：http://jta.fzhhl.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oai.zdqjudy.top

[R59] 发 POST JSON
来源：http://inq.dashuyun.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://swm.ehwqpu.com

[R60] 只看 HTTP 状态码
来源：http://mye.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wyp.xinyue.icu

[R61] 磁盘占用
来源：http://omy.0kj1m.cn

df -h;  du -sh *
来源：http://qlo.xingfuxueyuan.xyz

[R62] 找最占空间的文件
来源：http://dnh.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://kwl.xuetiantiany.cn

[R63] 内存与进程
来源：http://xer.yueranfly.top

free -h;  ps aux | grep nginx
来源：http://aqa.jqgfzy.top

[R64] 结束进程
来源：http://lxj.tanke756.top

kill -9 $(pgrep -f app.py)
来源：http://adp.9152youxi.cn

[R65] 查看端口占用
来源：http://mho.feifeiyinyue.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qws.ehwqpu.com

[R66] 定时任务
来源：http://svq.jqgfzy.top

crontab -e;  crontab -l
来源：http://lex.xinyue.icu

[R67] 生成随机十六进制串
来源：http://pzs.uphjek.com

openssl rand -hex 16
来源：http://hui.yj20258.top

[R68] 计算文件校验值
来源：http://eer.zhengqikj.top

sha256sum a.txt;  md5sum a.txt
来源：http://pqg.havefunace.top

[R69] 生成随机密码
来源：http://oly.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://fvo.guowangkeji.top

[R70] 时间戳与互转
来源：http://znl.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://pnv.fengsongda.top

[R71] 日期格式化
来源：http://bsi.shangyingyoupin.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://itk.jinqigufen.top

[R72] 等待端口就绪
来源：http://qlm.nanxuanxn.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jgl.jqgfzy.top

[R73] 分割大日志
来源：http://fcj.hysaishi.cn

split -l 1000 big.log part_
来源：http://vct.shangyingyoupin.top

[R74] 批量重命名
来源：http://dax.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bry.yonumen.top

[R75] 导出环境变量
来源：http://nxq.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://wgx.havefunace.top

[R76] 使用临时文件
来源：http://zdu.316326.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qbt.xuanzx.com

[R77] 读取用户输入
来源：http://zwv.chenzaomai.com

read -rp "请输入: " ans
来源：http://nsc.xuetiantiany.cn

[R78] 交互式菜单
来源：http://kfs.tianlin.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://pzj.yuanzhike.top

[R79] 解析命令行选项
来源：http://mks.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://enj.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://jen.pycfn.com

time ./run.sh
来源：http://jls.jinyuanbaomall.cn

================================================================================
来源：http://lny.vehdjk.com

S. C / C++ 专题
来源：http://pxy.redwolf501.top

================================================================================
来源：http://cyi.jqgfzy.top

[S01] C：Hello World
来源：http://uye.daria6918.cn

#include <stdio.h>
来源：http://imp.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tuq.tianlin.xyz

[S02] C：变量与格式化输出
来源：http://suz.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://loc.zhengqikj.top

[S03] C：读入整数
来源：http://lbo.guowangkeji.top

int x; scanf("%d", &x);
来源：http://sra.hongshengwenyu.top

[S04] C：字符串复制
来源：http://pva.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://dss.shzxlz.cn

[S05] C：字符串长度
来源：http://rvs.iojbl.cn

strlen(s)
来源：http://aba.tanke756.top

[S06] C：字符串比较
来源：http://nle.epnwcf.com

strcmp(a, b) == 0
来源：http://aid.andypj.xyz

[S07] C：数组遍历求和
来源：http://avh.0kj1m.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mdl.zhixingplan.top

[S08] C：动态内存分配与释放
来源：http://wky.9152youxi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tbd.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://wdu.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qcz.c1oappe.top

[S10] C：指针与解引用
来源：http://vur.316326.xyz

int *p = &a;  *p = 5;
来源：http://grg.yuanzhike.top

[S11] C：逐行读文件
来源：http://rjp.0kj1m.cn

FILE *f = fopen("a.txt", "r");
来源：http://nwe.shuidangran.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://skg.chenlongwang.top

fclose(f);
来源：http://gxf.bjfxy.top

[S12] C：写文件
来源：http://dwi.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vsx.sysykeji.top

[S13] C：宏定义
来源：http://dkb.xziqi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lkc.yvedp.cn

[S14] C：枚举
来源：http://mtr.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://nkl.nanxuanxn.top

[S15] C：类型转换
来源：http://mfi.dianchejie.cn

(double) a / b
来源：http://khu.yj20258888.top

[S16] C：位操作置位
来源：http://xnc.zhengqikj.top

x |= (1 << 3);
来源：http://fnm.zhaomingkeji.xyz

[S17] C：安全拼接字符串
来源：http://lii.guowangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://auy.guowangkeji.top

[S18] C：命令行参数
来源：http://meh.ctjpmb.com


<!-- 参考信息 -->